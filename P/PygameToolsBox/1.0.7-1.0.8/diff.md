# Comparing `tmp/PygameToolsBox-1.0.7.tar.gz` & `tmp/PygameToolsBox-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PygameToolsBox-1.0.7.tar", last modified: Sat Apr  6 19:36:27 2024, max compression
+gzip compressed data, was "PygameToolsBox-1.0.8.tar", last modified: Sat Apr  6 19:52:25 2024, max compression
```

## Comparing `PygameToolsBox-1.0.7.tar` & `PygameToolsBox-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 19:36:27.858291 PygameToolsBox-1.0.7/
--rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     3759 2024-04-06 19:36:27.857290 PygameToolsBox-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 19:36:27.825289 PygameToolsBox-1.0.7/PygameToolsBox/
--rw-rw-rw-   0        0        0       21 2024-04-06 19:36:14.000000 PygameToolsBox-1.0.7/PygameToolsBox/__init__.py
--rw-rw-rw-   0        0        0     4913 2024-04-06 19:27:29.000000 PygameToolsBox-1.0.7/PygameToolsBox/animated_object.py
--rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.7/PygameToolsBox/mask_image.py
--rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.7/PygameToolsBox/parallax_bg.py
--rw-rw-rw-   0        0        0     3696 2024-04-06 19:08:25.000000 PygameToolsBox-1.0.7/PygameToolsBox/spritesheet.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:36:27.855292 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/
--rw-rw-rw-   0        0        0     3759 2024-04-06 19:36:27.000000 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-06 19:36:27.000000 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 19:36:27.000000 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-06 19:36:27.000000 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-06 19:36:27.000000 PygameToolsBox-1.0.7/PygameToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3153 2024-04-06 19:35:17.000000 PygameToolsBox-1.0.7/README.md
--rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 19:36:27.858291 PygameToolsBox-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 19:52:25.105299 PygameToolsBox-1.0.8/
+-rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3749 2024-04-06 19:52:25.102993 PygameToolsBox-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 19:52:25.063366 PygameToolsBox-1.0.8/PygameToolsBox/
+-rw-rw-rw-   0        0        0       21 2024-04-06 19:52:11.000000 PygameToolsBox-1.0.8/PygameToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     5025 2024-04-06 19:48:59.000000 PygameToolsBox-1.0.8/PygameToolsBox/animated_object.py
+-rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.8/PygameToolsBox/mask_image.py
+-rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.8/PygameToolsBox/parallax_bg.py
+-rw-rw-rw-   0        0        0     3696 2024-04-06 19:08:25.000000 PygameToolsBox-1.0.8/PygameToolsBox/spritesheet.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:52:25.091991 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     3749 2024-04-06 19:52:25.000000 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-06 19:52:25.000000 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 19:52:25.000000 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-06 19:52:25.000000 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-06 19:52:25.000000 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3143 2024-04-06 19:50:04.000000 PygameToolsBox-1.0.8/README.md
+-rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 19:52:25.105805 PygameToolsBox-1.0.8/setup.cfg
```

### Comparing `PygameToolsBox-1.0.7/LICENSE` & `PygameToolsBox-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.7/PKG-INFO` & `PygameToolsBox-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -97,13 +97,13 @@
     player.set_action("run")
 
     while(run):
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 run = False
 
-        rect = player.rect
-        #Adjust rect to new coordinates
-        player.update(Rect(100, 100, 60, 60))
+        pos = player.pos
+        #Adjust position to new coordinates
+        player.update(player.pos)
         player.draw(win)
 
         pygame.display.update()
```

### Comparing `PygameToolsBox-1.0.7/PygameToolsBox/animated_object.py` & `PygameToolsBox-1.0.8/PygameToolsBox/animated_object.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import itertools
 
 import pygame.sprite
-from pygame import Surface, Rect
+from pygame import Surface, Rect, Vector2
 from pygame.event import Event
 
 from PygameToolsBox.mask_image import MaskImage
 
 ANIMATION_END = pygame.USEREVENT + 99
 
 
@@ -61,14 +61,15 @@
         """
         self.images = [MaskImage(i) for i in images]
         self._actions = dict[str, ActionSequence]()
         self._current_action: ActionSequence | None = None
         self._current_image = self.images[0]
         self.cooling = cooling
         self.cool_down = cooling
+        self._pos = Vector2(0, 0)
 
     def add_action(self, name: str, repeat: int, index_start: int, index_end: int):
         """
         Define action for further call
         :param name: Name of the action (suggest to use Enum to simplify)
         :param repeat: Number of time to repeat the animation before end. Set to -1 to infinite loop
         :param index_start: Index in the list of the first image
@@ -90,26 +91,26 @@
     def get_action(self) -> str | None:
         """
         :return: Action currently set otherwise return None
         """
         return self._current_action.name if self._current_action else None
 
     @property
-    def rect(self) -> Rect:
+    def pos(self) -> Vector2:
         """
         :return: Rectangle of the current position of the sprite
         """
-        return self._current_image.rect
+        return self._pos
 
-    def update(self, rect: Rect):
+    def update(self, pos: Vector2):
         """
         Call every frame for adjust animation and object position
-        :param rect: New position for the sprite
+        :param pos: New position for the sprite
         """
-        self._current_image.rect.center = rect.center
+        self._pos = pos
 
         if self.cool_down > 0:
             self.cool_down -= 1
             return
 
         self.cool_down = self.cooling
         action_sequence = self._current_action.get_next()
@@ -119,19 +120,21 @@
             self._current_image = None
 
     def is_collide_with(self, other: MaskImage):
         """
         :param other: The other object (sprite) to test collision
         :return: True if the object is colliding with another object else return False
         """
+        self._current_image.rect.center = self._pos
         if self._current_image and pygame.sprite.collide_rect(self._current_image, other):
             if pygame.sprite.collide_mask(self._current_image, other):
                 return True
         return False
 
     def draw(self, win: Surface):
         """
         Display object to the screen
         :param win: Surface to draw
         """
         if self._current_image:
+            self._current_image.rect.center = self._pos
             win.blit(self._current_image.image, self._current_image.rect)
```

### Comparing `PygameToolsBox-1.0.7/PygameToolsBox/parallax_bg.py` & `PygameToolsBox-1.0.8/PygameToolsBox/parallax_bg.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.7/PygameToolsBox/spritesheet.py` & `PygameToolsBox-1.0.8/PygameToolsBox/spritesheet.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.7/PygameToolsBox.egg-info/PKG-INFO` & `PygameToolsBox-1.0.8/PygameToolsBox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -97,13 +97,13 @@
     player.set_action("run")
 
     while(run):
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 run = False
 
-        rect = player.rect
-        #Adjust rect to new coordinates
-        player.update(Rect(100, 100, 60, 60))
+        pos = player.pos
+        #Adjust position to new coordinates
+        player.update(player.pos)
         player.draw(win)
 
         pygame.display.update()
```

### Comparing `PygameToolsBox-1.0.7/README.md` & `PygameToolsBox-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,13 +81,13 @@
     player.set_action("run")
 
     while(run):
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 run = False
 
-        rect = player.rect
-        #Adjust rect to new coordinates
-        player.update(Rect(100, 100, 60, 60))
+        pos = player.pos
+        #Adjust position to new coordinates
+        player.update(player.pos)
         player.draw(win)
 
         pygame.display.update()
```

### Comparing `PygameToolsBox-1.0.7/pyproject.toml` & `PygameToolsBox-1.0.8/pyproject.toml`

 * *Files identical despite different names*

