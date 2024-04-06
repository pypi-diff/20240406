# Comparing `tmp/PygameToolsBox-1.0.6.tar.gz` & `tmp/PygameToolsBox-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PygameToolsBox-1.0.6.tar", last modified: Sat Apr  6 18:13:38 2024, max compression
+gzip compressed data, was "PygameToolsBox-1.0.7.tar", last modified: Sat Apr  6 19:36:27 2024, max compression
```

## Comparing `PygameToolsBox-1.0.6.tar` & `PygameToolsBox-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 18:13:38.688039 PygameToolsBox-1.0.6/
--rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     2524 2024-04-06 18:13:38.687037 PygameToolsBox-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 18:13:38.634621 PygameToolsBox-1.0.6/PygameToolsBox/
--rw-rw-rw-   0        0        0       21 2024-04-06 18:13:13.000000 PygameToolsBox-1.0.6/PygameToolsBox/__init__.py
--rw-rw-rw-   0        0        0     3221 2024-04-06 18:11:51.000000 PygameToolsBox-1.0.6/PygameToolsBox/animated_object.py
--rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.6/PygameToolsBox/mask_image.py
--rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.6/PygameToolsBox/parallax_bg.py
--rw-rw-rw-   0        0        0     3691 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.6/PygameToolsBox/spritesheet.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:13:38.675035 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/
--rw-rw-rw-   0        0        0     2524 2024-04-06 18:13:38.000000 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-06 18:13:38.000000 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 18:13:38.000000 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-06 18:13:38.000000 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-06 18:13:38.000000 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1918 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.6/README.md
--rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 18:13:38.688039 PygameToolsBox-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 19:36:27.858291 PygameToolsBox-1.0.7/
+-rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3759 2024-04-06 19:36:27.857290 PygameToolsBox-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 19:36:27.825289 PygameToolsBox-1.0.7/PygameToolsBox/
+-rw-rw-rw-   0        0        0       21 2024-04-06 19:36:14.000000 PygameToolsBox-1.0.7/PygameToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     4913 2024-04-06 19:27:29.000000 PygameToolsBox-1.0.7/PygameToolsBox/animated_object.py
+-rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.7/PygameToolsBox/mask_image.py
+-rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.7/PygameToolsBox/parallax_bg.py
+-rw-rw-rw-   0        0        0     3696 2024-04-06 19:08:25.000000 PygameToolsBox-1.0.7/PygameToolsBox/spritesheet.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:36:27.855292 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     3759 2024-04-06 19:36:27.000000 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-06 19:36:27.000000 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 19:36:27.000000 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-06 19:36:27.000000 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-06 19:36:27.000000 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3153 2024-04-06 19:35:17.000000 PygameToolsBox-1.0.7/README.md
+-rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 19:36:27.858291 PygameToolsBox-1.0.7/setup.cfg
```

### Comparing `PygameToolsBox-1.0.6/LICENSE` & `PygameToolsBox-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.6/PygameToolsBox/parallax_bg.py` & `PygameToolsBox-1.0.7/PygameToolsBox/parallax_bg.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.6/PygameToolsBox/spritesheet.py` & `PygameToolsBox-1.0.7/PygameToolsBox/spritesheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import pygame
 from pygame import Surface
 
 
 class SpriteSheet:
     def __init__(self,
                  sprite_sheet_path: Path,
-                 sprite_size_x: int,
-                 sprite_size_y: int,
+                 sprite_size_x: float,
+                 sprite_size_y: float,
                  nb_rows: int,
                  nb_cols: int,
                  alpha: bool = True):
         """
         :param sprite_sheet_path:
             Path and file of the spead sheet
             All sprites of the sprite sheet must be relative to same purpose.
@@ -76,15 +76,15 @@
 
     def get_sprite_range(self, start: [int, int], stop: [int, int]) -> [Surface]:
         """
         Return list of sub sprites for row, col start to row col end
         the start and end is included into set
         the index ins 0 based range
         :param start: (row, col) to start
-        :param end: (row, col) to end
+        :param stop: (row, col) to end
         :return:
         """
         index_start = start[0] * 100 + start[1]
         index_stop = stop[0] * 100 + stop[1]
         for row in range(start[0], stop[0] + 1):
             for col in range(self._cols):
                 if index_start <= row * 100 + col <= index_stop:
```

### Comparing `PygameToolsBox-1.0.6/pyproject.toml` & `PygameToolsBox-1.0.7/pyproject.toml`

 * *Files identical despite different names*

