# Comparing `tmp/pybud-gui-0.9.3.tar.gz` & `tmp/pybud-gui-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybud-gui-0.9.3.tar", last modified: Sat Apr  6 18:24:18 2024, max compression
+gzip compressed data, was "pybud-gui-0.9.4.tar", last modified: Sat Apr  6 18:45:33 2024, max compression
```

## Comparing `pybud-gui-0.9.3.tar` & `pybud-gui-0.9.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 18:24:18.495313 pybud-gui-0.9.3/
--rw-rw-rw-   0        0        0     4196 2024-04-06 18:24:18.494312 pybud-gui-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     3768 2024-04-06 18:19:35.000000 pybud-gui-0.9.3/README.md
--rw-rw-rw-   0        0        0      560 2024-04-06 18:24:10.000000 pybud-gui-0.9.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 18:24:18.495313 pybud-gui-0.9.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-06 18:24:18.456262 pybud-gui-0.9.3/src/
--rw-rw-rw-   0        0        0     2352 2024-03-28 12:56:03.000000 pybud-gui-0.9.3/src/example1.py
--rw-rw-rw-   0        0        0     3579 2024-03-28 19:49:41.000000 pybud-gui-0.9.3/src/example2.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:24:18.458263 pybud-gui-0.9.3/src/pybud/
--rw-rw-rw-   0        0        0     5407 2024-03-28 12:00:12.000000 pybud-gui-0.9.3/src/pybud/ansi.py
--rw-rw-rw-   0        0        0    18794 2024-03-28 13:09:35.000000 pybud-gui-0.9.3/src/pybud/drawer.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:24:18.461262 pybud-gui-0.9.3/src/pybud/gui/
--rw-rw-rw-   0        0        0     7466 2024-03-28 13:18:01.000000 pybud-gui-0.9.3/src/pybud/gui/gui.py
--rw-rw-rw-   0        0        0     1908 2024-03-28 09:48:29.000000 pybud-gui-0.9.3/src/pybud/gui/utils.py
--rw-rw-rw-   0        0        0    10030 2024-03-28 19:30:17.000000 pybud-gui-0.9.3/src/pybud/gui/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:24:18.478263 pybud-gui-0.9.3/src/pybud_gui.egg-info/
--rw-rw-rw-   0        0        0     4196 2024-04-06 18:24:18.000000 pybud-gui-0.9.3/src/pybud_gui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-06 18:24:18.000000 pybud-gui-0.9.3/src/pybud_gui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 18:24:18.000000 pybud-gui-0.9.3/src/pybud_gui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-06 18:24:18.000000 pybud-gui-0.9.3/src/pybud_gui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-06 18:24:18.000000 pybud-gui-0.9.3/src/pybud_gui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 18:45:33.962335 pybud-gui-0.9.4/
+-rw-rw-rw-   0        0        0     4156 2024-04-06 18:45:33.961336 pybud-gui-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3728 2024-04-06 18:44:39.000000 pybud-gui-0.9.4/README.md
+-rw-rw-rw-   0        0        0      560 2024-04-06 18:44:58.000000 pybud-gui-0.9.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 18:45:33.962335 pybud-gui-0.9.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 18:45:33.931413 pybud-gui-0.9.4/src/
+-rw-rw-rw-   0        0        0     2352 2024-03-28 12:56:03.000000 pybud-gui-0.9.4/src/example1.py
+-rw-rw-rw-   0        0        0     3579 2024-03-28 19:49:41.000000 pybud-gui-0.9.4/src/example2.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:45:33.933413 pybud-gui-0.9.4/src/pybud/
+-rw-rw-rw-   0        0        0     5407 2024-03-28 12:00:12.000000 pybud-gui-0.9.4/src/pybud/ansi.py
+-rw-rw-rw-   0        0        0    18794 2024-03-28 13:09:35.000000 pybud-gui-0.9.4/src/pybud/drawer.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:45:33.937415 pybud-gui-0.9.4/src/pybud/gui/
+-rw-rw-rw-   0        0        0     7466 2024-03-28 13:18:01.000000 pybud-gui-0.9.4/src/pybud/gui/gui.py
+-rw-rw-rw-   0        0        0     1908 2024-03-28 09:48:29.000000 pybud-gui-0.9.4/src/pybud/gui/utils.py
+-rw-rw-rw-   0        0        0    10030 2024-03-28 19:30:17.000000 pybud-gui-0.9.4/src/pybud/gui/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:45:33.959337 pybud-gui-0.9.4/src/pybud_gui.egg-info/
+-rw-rw-rw-   0        0        0     4156 2024-04-06 18:45:33.000000 pybud-gui-0.9.4/src/pybud_gui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-06 18:45:33.000000 pybud-gui-0.9.4/src/pybud_gui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 18:45:33.000000 pybud-gui-0.9.4/src/pybud_gui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-06 18:45:33.000000 pybud-gui-0.9.4/src/pybud_gui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-06 18:45:33.000000 pybud-gui-0.9.4/src/pybud_gui.egg-info/top_level.txt
```

### Comparing `pybud-gui-0.9.3/PKG-INFO` & `pybud-gui-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybud-gui
-Version: 0.9.3
+Version: 0.9.4
 Summary: Create beautiful console GUIs in python, using Widgets, Dialouges, and more!
 Author-email: Amirali Mollaei <aamproducts@gmail.com>
 License: BSD 4-clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -43,16 +43,15 @@
     ansi.flush()
     return "Awesome!"
 
 
 def main_dialouge(WIDTH=76):
     """ the main dialouge """
     # you can use `CStr`s to define colord text!
-    title = CStr("[") + CStr(" " + "PyBUD: GUI Beauty" +
-                             " ", forecolor=(255, 0, 0)) + CStr("]")
+    title = CStr("[") + CStr(" PyBUD: GUI Beauty ", forecolor=(255, 0, 0)) + CStr("]")
     # you can also use the built in str
     caption = "A python library for creating beautiful GUIs in console, with tons of diffrent components, such as Dialouges, Widgets, Drawables, color optimization, and more!"
     # initialize the main dialouge
     mydialouge = AutoDialouge(width=WIDTH, ctype=ColorType.LEGACY)
 
     mydialouge.add_widget(WidgetLabel(
         title,
```

### Comparing `pybud-gui-0.9.3/README.md` & `pybud-gui-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     ansi.flush()
     return "Awesome!"
 
 
 def main_dialouge(WIDTH=76):
     """ the main dialouge """
     # you can use `CStr`s to define colord text!
-    title = CStr("[") + CStr(" " + "PyBUD: GUI Beauty" +
-                             " ", forecolor=(255, 0, 0)) + CStr("]")
+    title = CStr("[") + CStr(" PyBUD: GUI Beauty ", forecolor=(255, 0, 0)) + CStr("]")
     # you can also use the built in str
     caption = "A python library for creating beautiful GUIs in console, with tons of diffrent components, such as Dialouges, Widgets, Drawables, color optimization, and more!"
     # initialize the main dialouge
     mydialouge = AutoDialouge(width=WIDTH, ctype=ColorType.LEGACY)
 
     mydialouge.add_widget(WidgetLabel(
         title,
```

### Comparing `pybud-gui-0.9.3/pyproject.toml` & `pybud-gui-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pybud-gui"
-version = "0.9.3"
+version = "0.9.4"
 dependencies = [
   "readchar==4.0.5",
 ]
 requires-python = ">= 3.10"
 authors = [
   {name = "Amirali Mollaei", email = "aamproducts@gmail.com"},
 ]
```

### Comparing `pybud-gui-0.9.3/src/example1.py` & `pybud-gui-0.9.4/src/example1.py`

 * *Files identical despite different names*

### Comparing `pybud-gui-0.9.3/src/example2.py` & `pybud-gui-0.9.4/src/example2.py`

 * *Files identical despite different names*

### Comparing `pybud-gui-0.9.3/src/pybud/ansi.py` & `pybud-gui-0.9.4/src/pybud/ansi.py`

 * *Files identical despite different names*

### Comparing `pybud-gui-0.9.3/src/pybud/drawer.py` & `pybud-gui-0.9.4/src/pybud/drawer.py`

 * *Files identical despite different names*

### Comparing `pybud-gui-0.9.3/src/pybud/gui/gui.py` & `pybud-gui-0.9.4/src/pybud/gui/gui.py`

 * *Files identical despite different names*

### Comparing `pybud-gui-0.9.3/src/pybud/gui/utils.py` & `pybud-gui-0.9.4/src/pybud/gui/utils.py`

 * *Files identical despite different names*

### Comparing `pybud-gui-0.9.3/src/pybud/gui/widgets.py` & `pybud-gui-0.9.4/src/pybud/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `pybud-gui-0.9.3/src/pybud_gui.egg-info/PKG-INFO` & `pybud-gui-0.9.4/src/pybud_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybud-gui
-Version: 0.9.3
+Version: 0.9.4
 Summary: Create beautiful console GUIs in python, using Widgets, Dialouges, and more!
 Author-email: Amirali Mollaei <aamproducts@gmail.com>
 License: BSD 4-clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -43,16 +43,15 @@
     ansi.flush()
     return "Awesome!"
 
 
 def main_dialouge(WIDTH=76):
     """ the main dialouge """
     # you can use `CStr`s to define colord text!
-    title = CStr("[") + CStr(" " + "PyBUD: GUI Beauty" +
-                             " ", forecolor=(255, 0, 0)) + CStr("]")
+    title = CStr("[") + CStr(" PyBUD: GUI Beauty ", forecolor=(255, 0, 0)) + CStr("]")
     # you can also use the built in str
     caption = "A python library for creating beautiful GUIs in console, with tons of diffrent components, such as Dialouges, Widgets, Drawables, color optimization, and more!"
     # initialize the main dialouge
     mydialouge = AutoDialouge(width=WIDTH, ctype=ColorType.LEGACY)
 
     mydialouge.add_widget(WidgetLabel(
         title,
```

