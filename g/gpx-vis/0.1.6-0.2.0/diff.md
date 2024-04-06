# Comparing `tmp/gpx_vis-0.1.6.tar.gz` & `tmp/gpx_vis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx_vis-0.1.6.tar", last modified: Fri Apr  5 15:11:34 2024, max compression
+gzip compressed data, was "gpx_vis-0.2.0.tar", last modified: Sat Apr  6 21:28:54 2024, max compression
```

## Comparing `gpx_vis-0.1.6.tar` & `gpx_vis-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 15:11:34.058030 gpx_vis-0.1.6/
--rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.1.6/LICENSE
--rw-r--r--   0 jwt        (501) staff       (20)     1250 2024-04-05 15:11:34.057156 gpx_vis-0.1.6/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      712 2024-04-05 15:10:14.000000 gpx_vis-0.1.6/README.md
--rw-r--r--   0 jwt        (501) staff       (20)      578 2024-04-05 14:42:31.000000 gpx_vis-0.1.6/pyproject.toml
--rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-05 15:11:34.058204 gpx_vis-0.1.6/setup.cfg
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 15:11:34.050822 gpx_vis-0.1.6/src/
--rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.1.6/src/__init__.py
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 15:11:34.056182 gpx_vis-0.1.6/src/gpx_vis.egg-info/
--rw-r--r--   0 jwt        (501) staff       (20)     1250 2024-04-05 15:11:32.000000 gpx_vis-0.1.6/src/gpx_vis.egg-info/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-05 15:11:32.000000 gpx_vis-0.1.6/src/gpx_vis.egg-info/SOURCES.txt
--rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-05 15:11:32.000000 gpx_vis-0.1.6/src/gpx_vis.egg-info/dependency_links.txt
--rw-r--r--   0 jwt        (501) staff       (20)       84 2024-04-05 15:11:32.000000 gpx_vis-0.1.6/src/gpx_vis.egg-info/requires.txt
--rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-05 15:11:32.000000 gpx_vis-0.1.6/src/gpx_vis.egg-info/top_level.txt
--rw-r--r--   0 jwt        (501) staff       (20)    17187 2024-04-05 15:09:58.000000 gpx_vis-0.1.6/src/gpx_vis.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-06 21:28:54.324493 gpx_vis-0.2.0/
+-rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.2.0/LICENSE
+-rw-r--r--   0 jwt        (501) staff       (20)     2312 2024-04-06 21:28:54.324103 gpx_vis-0.2.0/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)     1774 2024-04-06 21:28:30.000000 gpx_vis-0.2.0/README.md
+-rw-r--r--   0 jwt        (501) staff       (20)      578 2024-04-05 21:35:37.000000 gpx_vis-0.2.0/pyproject.toml
+-rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-06 21:28:54.325323 gpx_vis-0.2.0/setup.cfg
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-06 21:28:54.318631 gpx_vis-0.2.0/src/
+-rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.2.0/src/__init__.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-06 21:28:54.323579 gpx_vis-0.2.0/src/gpx_vis.egg-info/
+-rw-r--r--   0 jwt        (501) staff       (20)     2312 2024-04-06 21:28:54.000000 gpx_vis-0.2.0/src/gpx_vis.egg-info/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-06 21:28:54.000000 gpx_vis-0.2.0/src/gpx_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-06 21:28:54.000000 gpx_vis-0.2.0/src/gpx_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       84 2024-04-06 21:28:54.000000 gpx_vis-0.2.0/src/gpx_vis.egg-info/requires.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-06 21:28:54.000000 gpx_vis-0.2.0/src/gpx_vis.egg-info/top_level.txt
+-rw-r--r--   0 jwt        (501) staff       (20)    17387 2024-04-05 21:41:04.000000 gpx_vis-0.2.0/src/gpx_vis.py
```

### Comparing `gpx_vis-0.1.6/LICENSE` & `gpx_vis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx_vis-0.1.6/pyproject.toml` & `gpx_vis-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpx_vis"
-version = "0.1.6"
+version = "0.2.0"
 authors = [
   { name="Jia Wei Teh", email="jiaweiteh.astro@gmail.com" },
 ]
 description = "Plots your Komoot tours"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gpx_vis-0.1.6/src/gpx_vis.py` & `gpx_vis-0.2.0/src/gpx_vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 and are not very customisable. This hopefully solves the problem (a little).
 """
 # main library
 import gpxpy
 
 import os
 import math
+import branca
 import folium
 import numpy as np
 import pandas as pd
 import humanfriendly
 import cmasher as cmr
 import reverse_geocode
 import matplotlib.pyplot as plt
@@ -345,15 +346,17 @@
         # create popup
         popup = folium.Popup(iframe,
                      min_width=300,
                      max_width=300)
         # add tooltip
         tooltip = self._addTooltip(self, selected_idx)
         # add to group
-        folium.PolyLine(track_coords,
+        folium.ColorLine(track_coords,
+                        colors = self.z[ii:jj],
+                        colormap = branca.colormap.linear.viridis.scale(min(self.z),max(self.z)),
                         tooltip = tooltip,
                         weight = 4,
                         ).add_to(group)
         
         # add start/finish points
         folium.CircleMarker(location = track_coords[0],
                             radius = 5,
@@ -376,14 +379,15 @@
         highlight_line = {'geometry': {
                     'type': 'LineString',
                     # reverse coord from (y, x) into (x,y)
                     'coordinates': [coord[::-1] for coord in track_coords]
                     }}
         # add
         folium.features.GeoJson(
+                color = 'transparent',
                 data = highlight_line['geometry'],
                 control=False,
                 tooltip = tooltip,
                 highlight_function=highlight_function, 
                 ).add_to(group)
         
         return
```

