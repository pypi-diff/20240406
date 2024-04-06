# Comparing `tmp/pybureaucrat-1.0.1.tar.gz` & `tmp/pybureaucrat-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybureaucrat-1.0.1.tar", last modified: Mon Nov 20 18:29:46 2023, max compression
+gzip compressed data, was "pybureaucrat-1.0.4.tar", last modified: Sat Apr  6 04:10:32 2024, max compression
```

## Comparing `pybureaucrat-1.0.1.tar` & `pybureaucrat-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-11-20 18:29:46.490753 pybureaucrat-1.0.1/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-11-20 18:27:40.000000 pybureaucrat-1.0.1/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2023-11-20 18:27:40.000000 pybureaucrat-1.0.1/MANIFEST.in
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      775 2023-11-20 18:29:46.478753 pybureaucrat-1.0.1/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-11-20 18:27:40.000000 pybureaucrat-1.0.1/README.MD
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-11-20 18:29:46.470753 pybureaucrat-1.0.1/client/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-11-20 18:29:46.478753 pybureaucrat-1.0.1/client/common/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-31 21:37:13.000000 pybureaucrat-1.0.1/client/common/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2634 2023-10-31 21:37:13.000000 pybureaucrat-1.0.1/client/common/base.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1244 2023-11-04 01:02:07.000000 pybureaucrat-1.0.1/client/common/blobs.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      348 2023-11-20 18:27:40.000000 pybureaucrat-1.0.1/client/common/bureaucrat_connection.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      186 2023-10-31 21:37:13.000000 pybureaucrat-1.0.1/client/common/deserializers.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      813 2023-10-31 21:37:13.000000 pybureaucrat-1.0.1/client/common/queues.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1795 2023-11-04 16:18:26.000000 pybureaucrat-1.0.1/client/common/tables.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-11-20 18:29:46.478753 pybureaucrat-1.0.1/client/pybureaucrat.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      775 2023-11-20 18:29:46.000000 pybureaucrat-1.0.1/client/pybureaucrat.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      426 2023-11-20 18:29:46.000000 pybureaucrat-1.0.1/client/pybureaucrat.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-11-20 18:29:46.000000 pybureaucrat-1.0.1/client/pybureaucrat.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        7 2023-11-20 18:29:46.000000 pybureaucrat-1.0.1/client/pybureaucrat.egg-info/top_level.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-11-20 18:27:40.000000 pybureaucrat-1.0.1/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-11-20 18:29:46.490753 pybureaucrat-1.0.1/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1151 2023-11-20 18:27:40.000000 pybureaucrat-1.0.1/setup.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-11-20 18:27:40.000000 pybureaucrat-1.0.1/version.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      775 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/README.MD
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/client/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/client/common/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2634 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/base.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1244 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/blobs.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      348 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/bureaucrat_connection.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      186 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/deserializers.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      813 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/queues.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1795 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/tables.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/client/pybureaucrat.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      775 2024-04-06 04:10:32.000000 pybureaucrat-1.0.4/client/pybureaucrat.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      426 2024-04-06 04:10:32.000000 pybureaucrat-1.0.4/client/pybureaucrat.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2024-04-06 04:10:32.000000 pybureaucrat-1.0.4/client/pybureaucrat.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        7 2024-04-06 04:10:32.000000 pybureaucrat-1.0.4/client/pybureaucrat.egg-info/top_level.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1151 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/setup.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/version.txt
```

### Comparing `pybureaucrat-1.0.1/LICENSE` & `pybureaucrat-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.1/PKG-INFO` & `pybureaucrat-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybureaucrat
-Version: 1.0.1
+Version: 1.0.4
 Summary: A python client for bureaucrat server
 Home-page: https://github.com/LostSavannah/bureaucrat/tree/main/lib
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/pybureaucrat/issues
 Project-URL: Documentation, https://dev.moradev.dev/pybureaucrat/documentation
 Project-URL: Examples, https://dev.moradev.dev/pybureaucrat/examples
```

### Comparing `pybureaucrat-1.0.1/client/common/base.py` & `pybureaucrat-1.0.4/client/common/base.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.1/client/common/blobs.py` & `pybureaucrat-1.0.4/client/common/blobs.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.1/client/common/queues.py` & `pybureaucrat-1.0.4/client/common/queues.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.1/client/common/tables.py` & `pybureaucrat-1.0.4/client/common/tables.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.1/client/pybureaucrat.egg-info/PKG-INFO` & `pybureaucrat-1.0.4/client/pybureaucrat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybureaucrat
-Version: 1.0.1
+Version: 1.0.4
 Summary: A python client for bureaucrat server
 Home-page: https://github.com/LostSavannah/bureaucrat/tree/main/lib
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/pybureaucrat/issues
 Project-URL: Documentation, https://dev.moradev.dev/pybureaucrat/documentation
 Project-URL: Examples, https://dev.moradev.dev/pybureaucrat/examples
```

### Comparing `pybureaucrat-1.0.1/setup.py` & `pybureaucrat-1.0.4/setup.py`

 * *Files identical despite different names*

