# Comparing `tmp/cursesplus-3.6.tar.gz` & `tmp/cursesplus-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-3.6.tar", last modified: Sun Oct 29 16:07:43 2023, max compression
+gzip compressed data, was "cursesplus-3.6.2.tar", last modified: Sun Oct 29 23:20:06 2023, max compression
```

## Comparing `cursesplus-3.6.tar` & `cursesplus-3.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-10-29 16:07:43.606665 cursesplus-3.6/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-10-26 03:46:05.000000 cursesplus-3.6/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     5289 2023-10-29 16:07:43.606665 cursesplus-3.6/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     4724 2023-10-29 16:03:05.000000 cursesplus-3.6/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      621 2023-10-29 16:00:14.000000 cursesplus-3.6/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-10-29 16:07:43.606665 cursesplus-3.6/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-10-29 16:07:43.596665 cursesplus-3.6/src/
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-10-29 16:07:43.606665 cursesplus-3.6/src/cursesplus/
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1544 2023-10-29 16:07:27.000000 cursesplus-3.6/src/cursesplus/__init__.py
--rw-r--r--   0 jordan    (1000) jordan    (1000)      474 2023-10-27 16:05:52.000000 cursesplus-3.6/src/cursesplus/constants.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    25077 2023-10-26 15:57:07.000000 cursesplus-3.6/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    23190 2023-10-26 16:05:55.000000 cursesplus-3.6/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     9323 2023-10-26 15:57:26.000000 cursesplus-3.6/src/cursesplus/messagebox.py
--rw-r--r--   0 jordan    (1000) jordan    (1000)     3509 2023-10-26 03:46:05.000000 cursesplus-3.6/src/cursesplus/transitions.py
--rw-r--r--   0 jordan    (1000) jordan    (1000)     4808 2023-10-29 15:50:20.000000 cursesplus-3.6/src/cursesplus/tuibase.py
--rw-r--r--   0 jordan    (1000) jordan    (1000)     3064 2023-10-29 15:18:44.000000 cursesplus-3.6/src/cursesplus/utils.py
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1460 2023-10-29 15:23:49.000000 cursesplus-3.6/src/cursesplus/widgets.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-10-29 16:07:43.606665 cursesplus-3.6/src/cursesplus.egg-info/
--rw-r--r--   0 jordan    (1000) jordan    (1000)     5289 2023-10-29 16:07:43.000000 cursesplus-3.6/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      424 2023-10-29 16:07:43.000000 cursesplus-3.6/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-10-29 16:07:43.000000 cursesplus-3.6/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       11 2023-10-29 16:07:43.000000 cursesplus-3.6/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-10-29 23:20:06.729405 cursesplus-3.6.2/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-10-26 03:46:05.000000 cursesplus-3.6.2/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     5452 2023-10-29 23:20:06.729405 cursesplus-3.6.2/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     4885 2023-10-29 23:19:52.000000 cursesplus-3.6.2/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      623 2023-10-29 23:19:36.000000 cursesplus-3.6.2/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-10-29 23:20:06.729405 cursesplus-3.6.2/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-10-29 23:20:06.729405 cursesplus-3.6.2/src/
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-10-29 23:20:06.729405 cursesplus-3.6.2/src/cursesplus/
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1546 2023-10-29 23:04:22.000000 cursesplus-3.6.2/src/cursesplus/__init__.py
+-rw-r--r--   0 jordan    (1000) jordan    (1000)      474 2023-10-27 16:05:52.000000 cursesplus-3.6.2/src/cursesplus/constants.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    25077 2023-10-26 15:57:07.000000 cursesplus-3.6.2/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    23190 2023-10-26 16:05:55.000000 cursesplus-3.6.2/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     9323 2023-10-26 15:57:26.000000 cursesplus-3.6.2/src/cursesplus/messagebox.py
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     3509 2023-10-26 03:46:05.000000 cursesplus-3.6.2/src/cursesplus/transitions.py
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     5639 2023-10-29 23:18:36.000000 cursesplus-3.6.2/src/cursesplus/tuibase.py
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     3064 2023-10-29 15:18:44.000000 cursesplus-3.6.2/src/cursesplus/utils.py
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1664 2023-10-29 23:18:16.000000 cursesplus-3.6.2/src/cursesplus/widgets.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-10-29 23:20:06.729405 cursesplus-3.6.2/src/cursesplus.egg-info/
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     5452 2023-10-29 23:20:06.000000 cursesplus-3.6.2/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      424 2023-10-29 23:20:06.000000 cursesplus-3.6.2/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-10-29 23:20:06.000000 cursesplus-3.6.2/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       11 2023-10-29 23:20:06.000000 cursesplus-3.6.2/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-3.6/LICENSE` & `cursesplus-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-3.6/PKG-INFO` & `cursesplus-3.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 3.6
+Version: 3.6.2
 Summary: An advanced terminal-based UI library based off of curses
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,22 +31,34 @@
 
 cursesplus is getting a widgets based system. The old utilities have been moved to a classic class. filedialogues and message boxes remain. The program will likely be hard to use until everything is finalized.
 
 The new utilities are VERY object-oriented compared to the hybrid model of the old utilities.
 
 **DANGER: 3.x IS A TRULY BACKWARDS INCOMPATIBLE UPDATE. LOTS OF CODE WILL NEED TO BE REFACTORED!**
 
+### 3.6.2
+
+- Add global key events
+
+- Are called before widget key events
+
+- Syntax is the same
+
+- Add ability to remove key events once registered
+
 ### 3.6 - A Large Update of Events
 
 In 3.6, a series of new features have been announced. Things such as
 
 *Key Events*
 
 - All widgets now have an add_key_event method. This takes the key name (gotten with curses.keyname()) as well as a function and its args
 
+*UI Loops*
+
 - There is now a mainloop. BaseWindow.start_ui_loop()
 
 - It can be shut up quickly by adding a key event tied to BaseWindow.shut_up_ui_loop()
 
 # Documentation
 
 ## Two Ways to Use
```

### Comparing `cursesplus-3.6/README.md` & `cursesplus-3.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,34 @@
 
 cursesplus is getting a widgets based system. The old utilities have been moved to a classic class. filedialogues and message boxes remain. The program will likely be hard to use until everything is finalized.
 
 The new utilities are VERY object-oriented compared to the hybrid model of the old utilities.
 
 **DANGER: 3.x IS A TRULY BACKWARDS INCOMPATIBLE UPDATE. LOTS OF CODE WILL NEED TO BE REFACTORED!**
 
+### 3.6.2
+
+- Add global key events
+
+- Are called before widget key events
+
+- Syntax is the same
+
+- Add ability to remove key events once registered
+
 ### 3.6 - A Large Update of Events
 
 In 3.6, a series of new features have been announced. Things such as
 
 *Key Events*
 
 - All widgets now have an add_key_event method. This takes the key name (gotten with curses.keyname()) as well as a function and its args
 
+*UI Loops*
+
 - There is now a mainloop. BaseWindow.start_ui_loop()
 
 - It can be shut up quickly by adding a key event tied to BaseWindow.shut_up_ui_loop()
 
 # Documentation
 
 ## Two Ways to Use
```

### Comparing `cursesplus-3.6/pyproject.toml` & `cursesplus-3.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "3.6"
+version = "3.6.2"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An advanced terminal-based UI library based off of curses"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-3.6/src/cursesplus/__init__.py` & `cursesplus-3.6.2/src/cursesplus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 cursesplus.utils                Partially auto imported. Contains misc utility functions and classes that are used frequently
 
 cursesplus.widgets              Auto imported. Contains widget classes for 3.x
 
 NOTICE! CP UTILITIES ARE COMPLETELY INCOMPATIBLE WITH TUIBASE. TO USE THEM, CALL your BaseWindows.screen for the stdscr argument.
 """
 
-__version__ = "3.6"
+__version__ = "3.6.1"
 __author__ = "Enderbyte Programs"
 __package__ = "cursesplus"
 
 from .tuibase import *
 from . import transitions
 from . import filedialog
 from .widgets import *
```

### Comparing `cursesplus-3.6/src/cursesplus/cp.py` & `cursesplus-3.6.2/src/cursesplus/cp.py`

 * *Files identical despite different names*

### Comparing `cursesplus-3.6/src/cursesplus/filedialog.py` & `cursesplus-3.6.2/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-3.6/src/cursesplus/messagebox.py` & `cursesplus-3.6.2/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-3.6/src/cursesplus/transitions.py` & `cursesplus-3.6.2/src/cursesplus/transitions.py`

 * *Files identical despite different names*

### Comparing `cursesplus-3.6/src/cursesplus/tuibase.py` & `cursesplus-3.6.2/src/cursesplus/tuibase.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,34 +23,46 @@
         self.size_x, self.size_y = os.get_terminal_size()
         self.size_y -= 2
         self.size_x -= 1
         self.tui_window = Window(self,self.screen,self.size_x,self.size_y,0,0)
         self.tui_window.drawWindowBoundary = False
         self.tui_window.title = "Application"
         self.haltuiloop = False
+        self.master_key_events = {}
         
         #self.tui_window.update()
+    def add_key_event(self,keyname:str,func,args=()):
+        """Add a new key event. A key event is a functiom that is called when a key is pressed."""
+        self.master_key_events[keyname] = utils.CallableFunction(func,args)
+    def handle_key_events(self,keyname:str):
+        """Do all global key events based on the provided keyname"""
+        for c in list(self.master_key_events.items()):
+            if c[0] == keyname:
+                c[1].execute()
     def create_child_window(self,offset:utils.Coord,size:utils.Coord):
         """Create and return a new child Window object to your specification"""
         return Window(self,self.screen,size.x,size.y,offset.x,offset.y)
     def update(self):
         """Update and refresh the screen"""
         for w in self.children:
             w.update()
         self.screen.refresh()
     def update_keyevents(self,key:str):
         """Execute key event updates for all child windows"""
+        self.handle_key_events(key)
         for w in self.children:
             w.upadte_keyevents(key)
     def shut_up_ui_loop(self):
         """Shut down the UI loop"""
         self.haltuiloop = True
     def set_title(self,new_title:str):
         """Change the master window title"""
         self.tui_window.title = new_title
+    def get_title(self) -> str:
+        return self.tui_window.title
     def get_underlying_window(self):
         """Return this window as a WindowObject. Must be used for putting widgets on to the base screen"""
         return self.tui_window
     def show_boundary(self):
         """Show the Window Boundary and title on the master window"""
         self.tui_window.drawWindowBoundary = True
     def hide_boundary(self):
@@ -60,14 +72,20 @@
         """Start an infinite loop of updating the UI on a keypress"""
         while not self.haltuiloop:
             self.update()
             ch = curses.keyname(self.screen.getch())
             self.update_keyevents(ch)
             self.screen.clear()
         self.haltuiloop = False#Reset so it is good for next time
+    def remove_key_event(self,key_to_remove):
+        """Remove any functions registered to `key_to_remove`"""
+        try:
+            del self.master_key_events[key_to_remove]
+        except:
+            pass
 
 class Window:
     drawWindowBoundary = True
     def __init__(self,parent:BaseWindow,screen,size_x: int,size_y:int,offset_x:int,offset_y:int,window_title="Window"):
         self.screen: curses._CursesWindow = screen
         self.parent: BaseWindow = parent
         self.title = window_title
```

### Comparing `cursesplus-3.6/src/cursesplus/utils.py` & `cursesplus-3.6.2/src/cursesplus/utils.py`

 * *Files identical despite different names*

### Comparing `cursesplus-3.6/src/cursesplus/widgets.py` & `cursesplus-3.6.2/src/cursesplus/widgets.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,20 @@
             activech = curses.keyname(key_as_int)
         else:
             activech = key_as_str
 
         for kv in list(self.key_events.items()):
             if activech == kv[0]:
                 kv[1].execute()
+    def remove_key_event(self,key_to_remove):
+        """Remove any functions registered to `key_to_remove`"""
+        try:
+            del self.key_events[key_to_remove]
+        except:
+            pass
 
 class Label(Control):
     def __init__(self,parent_window,location:utils.Coord,text:str,colour=0):
         super().__init__(parent_window,location)
         self.text = text
         self.is_selectable = False
         self.colour = colour
```

### Comparing `cursesplus-3.6/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-3.6.2/src/cursesplus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 3.6
+Version: 3.6.2
 Summary: An advanced terminal-based UI library based off of curses
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,22 +31,34 @@
 
 cursesplus is getting a widgets based system. The old utilities have been moved to a classic class. filedialogues and message boxes remain. The program will likely be hard to use until everything is finalized.
 
 The new utilities are VERY object-oriented compared to the hybrid model of the old utilities.
 
 **DANGER: 3.x IS A TRULY BACKWARDS INCOMPATIBLE UPDATE. LOTS OF CODE WILL NEED TO BE REFACTORED!**
 
+### 3.6.2
+
+- Add global key events
+
+- Are called before widget key events
+
+- Syntax is the same
+
+- Add ability to remove key events once registered
+
 ### 3.6 - A Large Update of Events
 
 In 3.6, a series of new features have been announced. Things such as
 
 *Key Events*
 
 - All widgets now have an add_key_event method. This takes the key name (gotten with curses.keyname()) as well as a function and its args
 
+*UI Loops*
+
 - There is now a mainloop. BaseWindow.start_ui_loop()
 
 - It can be shut up quickly by adding a key event tied to BaseWindow.shut_up_ui_loop()
 
 # Documentation
 
 ## Two Ways to Use
```

