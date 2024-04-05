# Comparing `tmp/floggit-0.0.8.tar.gz` & `tmp/floggit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floggit-0.0.8.tar", last modified: Wed Jan 31 09:00:15 2024, max compression
+gzip compressed data, was "floggit-0.0.9.tar", last modified: Thu Feb 15 05:59:47 2024, max compression
```

## Comparing `floggit-0.0.8.tar` & `floggit-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tim.eller   (504) staff       (20)        0 2024-01-31 09:00:15.066826 floggit-0.0.8/
--rw-r--r--   0 tim.eller   (504) staff       (20)      746 2024-01-31 09:00:15.066591 floggit-0.0.8/PKG-INFO
--rw-r--r--   0 tim.eller   (504) staff       (20)      976 2024-01-18 00:34:37.000000 floggit-0.0.8/README.md
-drwxr-xr-x   0 tim.eller   (504) staff       (20)        0 2024-01-31 09:00:15.065107 floggit-0.0.8/floggit/
--rw-r--r--   0 tim.eller   (504) staff       (20)       48 2024-01-31 08:59:02.000000 floggit-0.0.8/floggit/__init__.py
--rw-r--r--   0 tim.eller   (504) staff       (20)     4227 2024-01-18 18:04:14.000000 floggit-0.0.8/floggit/floggit.py
-drwxr-xr-x   0 tim.eller   (504) staff       (20)        0 2024-01-31 09:00:15.066384 floggit-0.0.8/floggit.egg-info/
--rw-r--r--   0 tim.eller   (504) staff       (20)      746 2024-01-31 09:00:15.000000 floggit-0.0.8/floggit.egg-info/PKG-INFO
--rw-r--r--   0 tim.eller   (504) staff       (20)      211 2024-01-31 09:00:15.000000 floggit-0.0.8/floggit.egg-info/SOURCES.txt
--rw-r--r--   0 tim.eller   (504) staff       (20)        1 2024-01-31 09:00:15.000000 floggit-0.0.8/floggit.egg-info/dependency_links.txt
--rw-r--r--   0 tim.eller   (504) staff       (20)       49 2024-01-31 09:00:15.000000 floggit-0.0.8/floggit.egg-info/requires.txt
--rw-r--r--   0 tim.eller   (504) staff       (20)        8 2024-01-31 09:00:15.000000 floggit-0.0.8/floggit.egg-info/top_level.txt
--rw-r--r--   0 tim.eller   (504) staff       (20)       38 2024-01-31 09:00:15.066866 floggit-0.0.8/setup.cfg
--rw-r--r--   0 tim.eller   (504) staff       (20)     1074 2024-01-31 08:58:51.000000 floggit-0.0.8/setup.py
+drwxr-xr-x   0 tim.eller   (504) staff       (20)        0 2024-02-15 05:59:47.898198 floggit-0.0.9/
+-rw-r--r--   0 tim.eller   (504) staff       (20)      746 2024-02-15 05:59:47.898000 floggit-0.0.9/PKG-INFO
+-rw-r--r--   0 tim.eller   (504) staff       (20)      976 2024-02-15 05:39:29.000000 floggit-0.0.9/README.md
+drwxr-xr-x   0 tim.eller   (504) staff       (20)        0 2024-02-15 05:59:47.897004 floggit-0.0.9/floggit/
+-rw-r--r--   0 tim.eller   (504) staff       (20)       48 2024-02-15 05:39:40.000000 floggit-0.0.9/floggit/__init__.py
+-rw-r--r--   0 tim.eller   (504) staff       (20)     4223 2024-02-15 05:40:46.000000 floggit-0.0.9/floggit/floggit.py
+drwxr-xr-x   0 tim.eller   (504) staff       (20)        0 2024-02-15 05:59:47.897823 floggit-0.0.9/floggit.egg-info/
+-rw-r--r--   0 tim.eller   (504) staff       (20)      746 2024-02-15 05:59:47.000000 floggit-0.0.9/floggit.egg-info/PKG-INFO
+-rw-r--r--   0 tim.eller   (504) staff       (20)      211 2024-02-15 05:59:47.000000 floggit-0.0.9/floggit.egg-info/SOURCES.txt
+-rw-r--r--   0 tim.eller   (504) staff       (20)        1 2024-02-15 05:59:47.000000 floggit-0.0.9/floggit.egg-info/dependency_links.txt
+-rw-r--r--   0 tim.eller   (504) staff       (20)       49 2024-02-15 05:59:47.000000 floggit-0.0.9/floggit.egg-info/requires.txt
+-rw-r--r--   0 tim.eller   (504) staff       (20)        8 2024-02-15 05:59:47.000000 floggit-0.0.9/floggit.egg-info/top_level.txt
+-rw-r--r--   0 tim.eller   (504) staff       (20)       38 2024-02-15 05:59:47.898244 floggit-0.0.9/setup.cfg
+-rw-r--r--   0 tim.eller   (504) staff       (20)     1074 2024-02-15 05:39:29.000000 floggit-0.0.9/setup.py
```

### Comparing `floggit-0.0.8/PKG-INFO` & `floggit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floggit
-Version: 0.0.8
+Version: 0.0.9
 Summary: log function inputs and outputs at runtime
 Home-page: https://github.com/dcyd-inc/floggit
 Author: dcyd, inc.
 Author-email: info@dcyd.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `floggit-0.0.8/README.md` & `floggit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `floggit-0.0.8/floggit/floggit.py` & `floggit-0.0.9/floggit/floggit.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             j.append(jsonify_payload(i))
         return j
     elif type(payload).__name__ == 'Response':
         return jsonify_payload(payload.get_json())
     elif type(payload).__name__ in ['DataFrame', 'Series']:
         return payload.head().to_json(
                 orient='split', default_handler=str, date_format='iso')
-    elif type(payload).__name__ == 'Graph':
+    elif isinstance(payload, nx.Graph):
         return json.dumps(nx.node_link_data(payload))
     elif type(payload).__name__ == 'set':
         return jsonify_payload(list(payload))
     else: # non-Response atomic type
         try:
             return jsonify_payload(dict(payload))
         except:
```

### Comparing `floggit-0.0.8/floggit.egg-info/PKG-INFO` & `floggit-0.0.9/floggit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floggit
-Version: 0.0.8
+Version: 0.0.9
 Summary: log function inputs and outputs at runtime
 Home-page: https://github.com/dcyd-inc/floggit
 Author: dcyd, inc.
 Author-email: info@dcyd.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `floggit-0.0.8/setup.py` & `floggit-0.0.9/setup.py`

 * *Files identical despite different names*

