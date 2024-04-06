# Comparing `tmp/redsauce-0.0.1.0.tar.gz` & `tmp/redsauce-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redsauce-0.0.1.0.tar", last modified: Fri Apr  5 00:26:35 2024, max compression
+gzip compressed data, was "redsauce-0.0.1.1.tar", last modified: Sat Apr  6 00:32:26 2024, max compression
```

## Comparing `redsauce-0.0.1.0.tar` & `redsauce-0.0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:26:35.372026 redsauce-0.0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-05 00:26:27.000000 redsauce-0.0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-05 00:26:35.372026 redsauce-0.0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 00:26:27.000000 redsauce-0.0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:26:35.372026 redsauce-0.0.1.0/redsauce/
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-05 00:26:27.000000 redsauce-0.0.1.0/redsauce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-05 00:26:27.000000 redsauce-0.0.1.0/redsauce/pickles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-05 00:26:27.000000 redsauce-0.0.1.0/redsauce/utensils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:26:35.372026 redsauce-0.0.1.0/redsauce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-05 00:26:35.000000 redsauce-0.0.1.0/redsauce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-05 00:26:35.000000 redsauce-0.0.1.0/redsauce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:26:35.000000 redsauce-0.0.1.0/redsauce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 00:26:35.000000 redsauce-0.0.1.0/redsauce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 00:26:35.000000 redsauce-0.0.1.0/redsauce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:26:35.372026 redsauce-0.0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-05 00:26:27.000000 redsauce-0.0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:32:26.116566 redsauce-0.0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-06 00:32:26.116566 redsauce-0.0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:32:26.116566 redsauce-0.0.1.1/redsauce/
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/redsauce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/redsauce/pickles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/redsauce/utensils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:32:26.116566 redsauce-0.0.1.1/redsauce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-06 00:32:26.000000 redsauce-0.0.1.1/redsauce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-06 00:32:26.000000 redsauce-0.0.1.1/redsauce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:32:26.000000 redsauce-0.0.1.1/redsauce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 00:32:26.000000 redsauce-0.0.1.1/redsauce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 00:32:26.000000 redsauce-0.0.1.1/redsauce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:32:26.116566 redsauce-0.0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/setup.py
```

### Comparing `redsauce-0.0.1.0/LICENSE` & `redsauce-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redsauce-0.0.1.0/redsauce/pickles.py` & `redsauce-0.0.1.1/redsauce/pickles.py`

 * *Files identical despite different names*

