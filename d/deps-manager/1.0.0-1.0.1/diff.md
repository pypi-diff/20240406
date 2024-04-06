# Comparing `tmp/deps-manager-1.0.0.tar.gz` & `tmp/deps-manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps-manager-1.0.0.tar", last modified: Sat Apr  6 02:29:48 2024, max compression
+gzip compressed data, was "deps-manager-1.0.1.tar", last modified: Sat Apr  6 04:41:18 2024, max compression
```

## Comparing `deps-manager-1.0.0.tar` & `deps-manager-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:29:48.317372 deps-manager-1.0.0/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      276 2024-04-06 02:29:48.317133 deps-manager-1.0.0/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)     1916 2024-04-06 02:20:53.000000 deps-manager-1.0.0/README.md
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:29:48.315791 deps-manager-1.0.0/deps_manager/
--rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.0/deps_manager/__init__.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     2615 2024-04-06 02:20:53.000000 deps-manager-1.0.0/deps_manager/dependencies.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     2465 2024-04-06 02:20:53.000000 deps-manager-1.0.0/deps_manager/main.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.0/deps_manager/utils.py
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:29:48.316798 deps-manager-1.0.0/deps_manager.egg-info/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      276 2024-04-06 02:29:48.000000 deps-manager-1.0.0/deps_manager.egg-info/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-04-06 02:29:48.000000 deps-manager-1.0.0/deps_manager.egg-info/SOURCES.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-04-06 02:29:48.000000 deps-manager-1.0.0/deps_manager.egg-info/dependency_links.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-04-06 02:29:48.000000 deps-manager-1.0.0/deps_manager.egg-info/entry_points.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)        6 2024-04-06 02:29:48.000000 deps-manager-1.0.0/deps_manager.egg-info/requires.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-04-06 02:29:48.000000 deps-manager-1.0.0/deps_manager.egg-info/top_level.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-04-06 02:29:48.317433 deps-manager-1.0.0/setup.cfg
--rw-r--r--   0 harshadatupe   (501) staff       (20)      535 2024-04-06 02:20:53.000000 deps-manager-1.0.0/setup.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-04-06 04:41:18.417679 deps-manager-1.0.1/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      276 2024-04-06 04:41:18.416859 deps-manager-1.0.1/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     1916 2024-04-06 02:20:53.000000 deps-manager-1.0.1/README.md
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-04-06 04:41:18.410192 deps-manager-1.0.1/deps_manager/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.1/deps_manager/__init__.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     2615 2024-04-06 02:20:53.000000 deps-manager-1.0.1/deps_manager/dependencies.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     2489 2024-04-06 04:38:08.000000 deps-manager-1.0.1/deps_manager/main.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.1/deps_manager/utils.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-04-06 04:41:18.415545 deps-manager-1.0.1/deps_manager.egg-info/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      276 2024-04-06 04:41:18.000000 deps-manager-1.0.1/deps_manager.egg-info/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-04-06 04:41:18.000000 deps-manager-1.0.1/deps_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-04-06 04:41:18.000000 deps-manager-1.0.1/deps_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-04-06 04:41:18.000000 deps-manager-1.0.1/deps_manager.egg-info/entry_points.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        6 2024-04-06 04:41:18.000000 deps-manager-1.0.1/deps_manager.egg-info/requires.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-04-06 04:41:18.000000 deps-manager-1.0.1/deps_manager.egg-info/top_level.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-04-06 04:41:18.417879 deps-manager-1.0.1/setup.cfg
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      535 2024-04-06 04:38:08.000000 deps-manager-1.0.1/setup.py
```

### Comparing `deps-manager-1.0.0/README.md` & `deps-manager-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `deps-manager-1.0.0/deps_manager/dependencies.py` & `deps-manager-1.0.1/deps_manager/dependencies.py`

 * *Files identical despite different names*

### Comparing `deps-manager-1.0.0/deps_manager/main.py` & `deps-manager-1.0.1/deps_manager/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     Decorator for the requirements file option.
     """
     return click.option('-r', '--requirements_file', prompt="Enter the requirements.txt file name", required=True,
                         help="Path to requirements file")(function)
 
 
 @click.group()
+@click.version_option()
 def cli():
     """Command Line Interface for managing project dependencies."""
     pass
 
 
 @cli.command()
 @common_options
```

### Comparing `deps-manager-1.0.0/setup.py` & `deps-manager-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='deps-manager',
-    version='1.0.0',
+    version='1.0.1',
     author="Harshada Tupe",
     author_email="harshadatupe8@gmail.com",
     license="MIT",
     packages=find_packages(),
     classifiers=["Programming Language :: Python :: 3 :: Only",
                  "Operating System :: OS Independent"],
     python_requires='>=3.8',
```

