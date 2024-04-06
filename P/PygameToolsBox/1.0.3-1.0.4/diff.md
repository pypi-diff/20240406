# Comparing `tmp/PygameToolsBox-1.0.3.tar.gz` & `tmp/PygameToolsBox-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PygameToolsBox-1.0.3.tar", last modified: Wed Apr  3 15:11:23 2024, max compression
+gzip compressed data, was "PygameToolsBox-1.0.4.tar", last modified: Sat Apr  6 17:39:37 2024, max compression
```

## Comparing `PygameToolsBox-1.0.3.tar` & `PygameToolsBox-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 15:11:23.619131 PygameToolsBox-1.0.3/
--rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2524 2024-04-03 15:11:23.618010 PygameToolsBox-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 15:11:23.594207 PygameToolsBox-1.0.3/PygameToolsBox/
--rw-rw-rw-   0        0        0       21 2024-04-03 15:10:42.000000 PygameToolsBox-1.0.3/PygameToolsBox/__init__.py
--rw-rw-rw-   0        0        0     3098 2024-04-03 15:09:03.000000 PygameToolsBox-1.0.3/PygameToolsBox/animated_object.py
--rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.3/PygameToolsBox/mask_image.py
--rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.3/PygameToolsBox/parallax_bg.py
--rw-rw-rw-   0        0        0     3691 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.3/PygameToolsBox/spritesheet.py
-drwxrwxrwx   0        0        0        0 2024-04-03 15:11:23.616969 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/
--rw-rw-rw-   0        0        0     2524 2024-04-03 15:11:23.000000 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-03 15:11:23.000000 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 15:11:23.000000 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-03 15:11:23.000000 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-03 15:11:23.000000 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1918 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.3/README.md
--rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 15:11:23.619131 PygameToolsBox-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 17:39:37.177484 PygameToolsBox-1.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2524 2024-04-06 17:39:37.176472 PygameToolsBox-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 17:39:37.146479 PygameToolsBox-1.0.4/PygameToolsBox/
+-rw-rw-rw-   0        0        0       21 2024-04-06 17:39:24.000000 PygameToolsBox-1.0.4/PygameToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     3194 2024-04-06 17:36:46.000000 PygameToolsBox-1.0.4/PygameToolsBox/animated_object.py
+-rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.4/PygameToolsBox/mask_image.py
+-rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.4/PygameToolsBox/parallax_bg.py
+-rw-rw-rw-   0        0        0     3691 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.4/PygameToolsBox/spritesheet.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:39:37.175473 PygameToolsBox-1.0.4/PygameToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     2524 2024-04-06 17:39:37.000000 PygameToolsBox-1.0.4/PygameToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-06 17:39:37.000000 PygameToolsBox-1.0.4/PygameToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 17:39:37.000000 PygameToolsBox-1.0.4/PygameToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-06 17:39:37.000000 PygameToolsBox-1.0.4/PygameToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-06 17:39:37.000000 PygameToolsBox-1.0.4/PygameToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1918 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.4/README.md
+-rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 17:39:37.178472 PygameToolsBox-1.0.4/setup.cfg
```

### Comparing `PygameToolsBox-1.0.3/LICENSE` & `PygameToolsBox-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.3/PKG-INFO` & `PygameToolsBox-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.0.3/PygameToolsBox/animated_object.py` & `PygameToolsBox-1.0.4/PygameToolsBox/animated_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,26 +64,31 @@
         if action in self._actions:
             self._current_action = self._actions[action]
             self._current_action.start()
 
     def get_action(self):
         return self._current_action.name
 
+    @property.getter
+    def rect(self) -> Rect:
+        return self._current_image.rect
+
     def update(self, rect: Rect):
+        self._current_image.rect.center = rect.center
+
         if self.cool_down > 0:
             self.cool_down -= 1
             return
 
         self.cool_down = self.cooling
         action_sequence = self._current_action.get_next()
         if action_sequence is not None:
             self._current_image = self.images[action_sequence]
         else:
             self._current_image = None
-        self._current_image.rect.center = rect.center
 
     def is_collide_with(self, other: MaskImage):
         if self._current_image and pygame.sprite.collide_rect(self._current_image, other):
             if pygame.sprite.collide_mask(self._current_image, other):
                 return True
         return False
```

### Comparing `PygameToolsBox-1.0.3/PygameToolsBox/parallax_bg.py` & `PygameToolsBox-1.0.4/PygameToolsBox/parallax_bg.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.3/PygameToolsBox/spritesheet.py` & `PygameToolsBox-1.0.4/PygameToolsBox/spritesheet.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.3/PygameToolsBox.egg-info/PKG-INFO` & `PygameToolsBox-1.0.4/PygameToolsBox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.0.3/README.md` & `PygameToolsBox-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.3/pyproject.toml` & `PygameToolsBox-1.0.4/pyproject.toml`

 * *Files identical despite different names*

