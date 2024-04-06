# Comparing `tmp/kv-api-0.1.1.tar.gz` & `tmp/kv-api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv-api-0.1.1.tar", last modified: Fri Apr  5 13:12:20 2024, max compression
+gzip compressed data, was "kv-api-0.1.2.tar", last modified: Sat Apr  6 08:35:39 2024, max compression
```

## Comparing `kv-api-0.1.1.tar` & `kv-api-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:12:20.700847 kv-api-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      292 2024-04-05 13:12:20.700847 kv-api-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv-api-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      520 2024-04-05 13:12:18.000000 kv-api-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-05 13:12:20.700847 kv-api-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:12:20.690847 kv-api-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:12:20.690847 kv-api-0.1.1/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:12:20.690847 kv-api-0.1.1/src/kv/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-04-05 12:42:30.000000 kv-api-0.1.1/src/kv/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1934 2024-04-05 12:42:30.000000 kv-api-0.1.1/src/kv/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:12:20.690847 kv-api-0.1.1/src/kv/api/asyncify/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-04-05 12:42:30.000000 kv-api-0.1.1/src/kv/api/asyncify/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1395 2024-04-05 12:42:30.000000 kv-api-0.1.1/src/kv/api/asyncify/asyncify.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:12:20.690847 kv-api-0.1.1/src/kv/api/errors/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       70 2024-04-05 12:42:30.000000 kv-api-0.1.1/src/kv/api/errors/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      613 2024-04-05 12:42:30.000000 kv-api-0.1.1/src/kv/api/errors/errors.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:12:20.690847 kv-api-0.1.1/src/kv_api.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      292 2024-04-05 13:12:20.000000 kv-api-0.1.1/src/kv_api.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      356 2024-04-05 13:12:20.000000 kv-api-0.1.1/src/kv_api.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-05 13:12:20.000000 kv-api-0.1.1/src/kv_api.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-05 13:12:20.000000 kv-api-0.1.1/src/kv_api.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-05 13:12:20.000000 kv-api-0.1.1/src/kv_api.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:35:39.433107 kv-api-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-06 08:35:39.433107 kv-api-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv-api-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      603 2024-04-06 08:35:37.000000 kv-api-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-06 08:35:39.433107 kv-api-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:35:39.423107 kv-api-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:35:39.423107 kv-api-0.1.2/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:35:39.423107 kv-api-0.1.2/src/kv/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-04-05 12:42:30.000000 kv-api-0.1.2/src/kv/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2153 2024-04-06 08:35:28.000000 kv-api-0.1.2/src/kv/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:35:39.423107 kv-api-0.1.2/src/kv/api/asyncify/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-04-05 12:42:30.000000 kv-api-0.1.2/src/kv/api/asyncify/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1395 2024-04-05 12:42:30.000000 kv-api-0.1.2/src/kv/api/asyncify/asyncify.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:35:39.423107 kv-api-0.1.2/src/kv/api/errors/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       70 2024-04-05 12:42:30.000000 kv-api-0.1.2/src/kv/api/errors/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      613 2024-04-05 12:42:30.000000 kv-api-0.1.2/src/kv/api/errors/errors.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:35:39.423107 kv-api-0.1.2/src/kv_api.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-06 08:35:39.000000 kv-api-0.1.2/src/kv_api.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      356 2024-04-06 08:35:39.000000 kv-api-0.1.2/src/kv_api.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-06 08:35:39.000000 kv-api-0.1.2/src/kv_api.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-06 08:35:39.000000 kv-api-0.1.2/src/kv_api.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-06 08:35:39.000000 kv-api-0.1.2/src/kv_api.egg-info/top_level.txt
```

### Comparing `kv-api-0.1.1/src/kv/api/asyncify/asyncify.py` & `kv-api-0.1.2/src/kv/api/asyncify/asyncify.py`

 * *Files identical despite different names*

### Comparing `kv-api-0.1.1/src/kv/api/errors/errors.py` & `kv-api-0.1.2/src/kv/api/errors/errors.py`

 * *Files identical despite different names*

