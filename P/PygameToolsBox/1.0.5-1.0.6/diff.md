# Comparing `tmp/PygameToolsBox-1.0.5.tar.gz` & `tmp/PygameToolsBox-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PygameToolsBox-1.0.5.tar", last modified: Sat Apr  6 17:57:35 2024, max compression
+gzip compressed data, was "PygameToolsBox-1.0.6.tar", last modified: Sat Apr  6 18:13:38 2024, max compression
```

## Comparing `PygameToolsBox-1.0.5.tar` & `PygameToolsBox-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 17:57:35.099604 PygameToolsBox-1.0.5/
--rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2524 2024-04-06 17:57:35.098595 PygameToolsBox-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 17:57:35.063243 PygameToolsBox-1.0.5/PygameToolsBox/
--rw-rw-rw-   0        0        0       21 2024-04-06 17:57:11.000000 PygameToolsBox-1.0.5/PygameToolsBox/__init__.py
--rw-rw-rw-   0        0        0     3187 2024-04-06 17:54:48.000000 PygameToolsBox-1.0.5/PygameToolsBox/animated_object.py
--rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.5/PygameToolsBox/mask_image.py
--rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.5/PygameToolsBox/parallax_bg.py
--rw-rw-rw-   0        0        0     3691 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.5/PygameToolsBox/spritesheet.py
-drwxrwxrwx   0        0        0        0 2024-04-06 17:57:35.087578 PygameToolsBox-1.0.5/PygameToolsBox.egg-info/
--rw-rw-rw-   0        0        0     2524 2024-04-06 17:57:35.000000 PygameToolsBox-1.0.5/PygameToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-06 17:57:35.000000 PygameToolsBox-1.0.5/PygameToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 17:57:35.000000 PygameToolsBox-1.0.5/PygameToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-06 17:57:35.000000 PygameToolsBox-1.0.5/PygameToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-06 17:57:35.000000 PygameToolsBox-1.0.5/PygameToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1918 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.5/README.md
--rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 17:57:35.099604 PygameToolsBox-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 18:13:38.688039 PygameToolsBox-1.0.6/
+-rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2524 2024-04-06 18:13:38.687037 PygameToolsBox-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 18:13:38.634621 PygameToolsBox-1.0.6/PygameToolsBox/
+-rw-rw-rw-   0        0        0       21 2024-04-06 18:13:13.000000 PygameToolsBox-1.0.6/PygameToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     3221 2024-04-06 18:11:51.000000 PygameToolsBox-1.0.6/PygameToolsBox/animated_object.py
+-rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.6/PygameToolsBox/mask_image.py
+-rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.6/PygameToolsBox/parallax_bg.py
+-rw-rw-rw-   0        0        0     3691 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.6/PygameToolsBox/spritesheet.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:13:38.675035 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     2524 2024-04-06 18:13:38.000000 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-06 18:13:38.000000 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 18:13:38.000000 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-06 18:13:38.000000 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-06 18:13:38.000000 PygameToolsBox-1.0.6/PygameToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1918 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.6/README.md
+-rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 18:13:38.688039 PygameToolsBox-1.0.6/setup.cfg
```

### Comparing `PygameToolsBox-1.0.5/LICENSE` & `PygameToolsBox-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.5/PKG-INFO` & `PygameToolsBox-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.0.5/PygameToolsBox/animated_object.py` & `PygameToolsBox-1.0.6/PygameToolsBox/animated_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     def set_action(self, action: str):
         if action in self._actions:
             self._current_action = self._actions[action]
             self._current_action.start()
 
     def get_action(self):
-        return self._current_action.name
+        return self._current_action.name if self._current_action else None
 
     @property
     def rect(self) -> Rect:
         return self._current_image.rect
 
     def update(self, rect: Rect):
         self._current_image.rect.center = rect.center
```

### Comparing `PygameToolsBox-1.0.5/PygameToolsBox/parallax_bg.py` & `PygameToolsBox-1.0.6/PygameToolsBox/parallax_bg.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.5/PygameToolsBox/spritesheet.py` & `PygameToolsBox-1.0.6/PygameToolsBox/spritesheet.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.5/PygameToolsBox.egg-info/PKG-INFO` & `PygameToolsBox-1.0.6/PygameToolsBox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.0.5/README.md` & `PygameToolsBox-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.5/pyproject.toml` & `PygameToolsBox-1.0.6/pyproject.toml`

 * *Files identical despite different names*

