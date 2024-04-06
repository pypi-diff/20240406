# Comparing `tmp/IS2view-0.0.6.tar.gz` & `tmp/IS2view-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IS2view-0.0.6.tar", last modified: Sat Mar 16 00:43:58 2024, max compression
+gzip compressed data, was "IS2view-0.0.7.tar", last modified: Sat Apr  6 18:00:33 2024, max compression
```

## Comparing `IS2view-0.0.6.tar` & `IS2view-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 00:43:58.252207 IS2view-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-16 00:43:47.000000 IS2view-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-03-16 00:43:47.000000 IS2view-0.0.6/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-16 00:43:47.000000 IS2view-0.0.6/CONTRIBUTORS.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 00:43:58.252207 IS2view-0.0.6/IS2view/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-16 00:43:47.000000 IS2view-0.0.6/IS2view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69070 2024-03-16 00:43:47.000000 IS2view-0.0.6/IS2view/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-03-16 00:43:47.000000 IS2view-0.0.6/IS2view/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-03-16 00:43:47.000000 IS2view-0.0.6/IS2view/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    18114 2024-03-16 00:43:47.000000 IS2view-0.0.6/IS2view/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    49704 2024-03-16 00:43:47.000000 IS2view-0.0.6/IS2view/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-16 00:43:47.000000 IS2view-0.0.6/IS2view/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 00:43:58.252207 IS2view-0.0.6/IS2view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-16 00:43:58.000000 IS2view-0.0.6/IS2view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-16 00:43:58.000000 IS2view-0.0.6/IS2view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 00:43:58.000000 IS2view-0.0.6/IS2view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-16 00:43:58.000000 IS2view-0.0.6/IS2view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-16 00:43:58.000000 IS2view-0.0.6/IS2view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-16 00:43:47.000000 IS2view-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-16 00:43:47.000000 IS2view-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-16 00:43:58.252207 IS2view-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-03-16 00:43:47.000000 IS2view-0.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-16 00:43:47.000000 IS2view-0.0.6/postBuild
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-16 00:43:47.000000 IS2view-0.0.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-16 00:43:47.000000 IS2view-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 00:43:58.252207 IS2view-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-16 00:43:47.000000 IS2view-0.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-16 00:43:47.000000 IS2view-0.0.6/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:00:33.866410 IS2view-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-06 18:00:23.000000 IS2view-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-06 18:00:23.000000 IS2view-0.0.7/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-06 18:00:23.000000 IS2view-0.0.7/CONTRIBUTORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:00:33.866410 IS2view-0.0.7/IS2view/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69246 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18114 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49704 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:00:33.866410 IS2view-0.0.7/IS2view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-06 18:00:33.000000 IS2view-0.0.7/IS2view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-06 18:00:33.000000 IS2view-0.0.7/IS2view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:00:33.000000 IS2view-0.0.7/IS2view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-06 18:00:33.000000 IS2view-0.0.7/IS2view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 18:00:33.000000 IS2view-0.0.7/IS2view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-06 18:00:23.000000 IS2view-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-06 18:00:23.000000 IS2view-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-06 18:00:33.866410 IS2view-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-06 18:00:23.000000 IS2view-0.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-06 18:00:23.000000 IS2view-0.0.7/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 18:00:23.000000 IS2view-0.0.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-06 18:00:23.000000 IS2view-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:00:33.866410 IS2view-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-06 18:00:23.000000 IS2view-0.0.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 18:00:23.000000 IS2view-0.0.7/version.txt
```

### Comparing `IS2view-0.0.6/.gitignore` & `IS2view-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.6/CODE_OF_CONDUCT.rst` & `IS2view-0.0.7/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.6/IS2view/__init__.py` & `IS2view-0.0.7/IS2view/__init__.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.6/IS2view/api.py` & `IS2view-0.0.7/IS2view/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,21 +193,29 @@
 def _load_dict(data):
     """Creates a xyzservices TileProvider object from a dictionary
     """
     providers = Bunch()
     for provider_name in data.keys():
         provider = data[provider_name]
         if "url" in provider.keys():
-            providers[provider_name] = xyzservices.lib.TileProvider(provider)
+            providers[provider_name] = _tile_provider(provider)
         else:
             providers[provider_name] = Bunch(
-                {i: xyzservices.lib.TileProvider(provider[i]) for i in provider.keys()}
+                {i: _tile_provider(provider[i]) for i in provider.keys()}
             )
     return providers
 
+def _tile_provider(provider):
+    """Creates a xyzservices TileProvider object
+    """
+    try:
+        return xyzservices.lib.TileProvider(provider)
+    except (NameError, AttributeError):
+        pass
+
 # create traitlets of basemap providers
 basemaps = _load_dict(providers)
 
 # draw ipyleaflet map
 class Leaflet:
     """Create interactive leaflet maps for visualizing ATL14/15 data
```

### Comparing `IS2view-0.0.6/IS2view/convert.py` & `IS2view-0.0.7/IS2view/convert.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.6/IS2view/io.py` & `IS2view-0.0.7/IS2view/io.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.6/IS2view/tools.py` & `IS2view-0.0.7/IS2view/tools.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.6/IS2view/utilities.py` & `IS2view-0.0.7/IS2view/utilities.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.6/IS2view.egg-info/PKG-INFO` & `IS2view-0.0.7/IS2view.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IS2view
-Version: 0.0.6
+Version: 0.0.7
 Summary: Interactive visualization and data extraction tool for the ICESat-2 ATL14/15 Gridded Land Ice Height Products
 Home-page: https://github.com/tsutterley/IS2view
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: ICESat-2,elevation,digital elevation models,ipython,jupyter,graphics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `IS2view-0.0.6/LICENSE` & `IS2view-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.6/PKG-INFO` & `IS2view-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IS2view
-Version: 0.0.6
+Version: 0.0.7
 Summary: Interactive visualization and data extraction tool for the ICESat-2 ATL14/15 Gridded Land Ice Height Products
 Home-page: https://github.com/tsutterley/IS2view
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: ICESat-2,elevation,digital elevation models,ipython,jupyter,graphics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `IS2view-0.0.6/README.rst` & `IS2view-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.6/setup.py` & `IS2view-0.0.7/setup.py`

 * *Files identical despite different names*

