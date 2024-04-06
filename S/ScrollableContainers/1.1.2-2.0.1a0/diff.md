# Comparing `tmp/ScrollableContainers-1.1.2.tar.gz` & `tmp/scrollablecontainers-2.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScrollableContainers-1.1.2.tar", last modified: Sat Sep 16 07:19:17 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ScrollableContainers-1.1.2.tar` & `scrollablecontainers-2.0.1a0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 tfpf      (1000) tfpf      (1000)        0 2023-09-16 07:19:17.741103 ScrollableContainers-1.1.2/
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)    31917 2023-05-21 21:11:52.000000 ScrollableContainers-1.1.2/COPYING.md
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)     4467 2023-09-16 07:19:17.737105 ScrollableContainers-1.1.2/PKG-INFO
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)     3891 2023-09-16 07:03:49.000000 ScrollableContainers-1.1.2/README.md
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)      648 2023-09-16 07:17:47.000000 ScrollableContainers-1.1.2/pyproject.toml
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)       38 2023-09-16 07:19:17.741103 ScrollableContainers-1.1.2/setup.cfg
-drwxr-xr-x   0 tfpf      (1000) tfpf      (1000)        0 2023-09-16 07:19:17.737105 ScrollableContainers-1.1.2/src/
-drwxr-xr-x   0 tfpf      (1000) tfpf      (1000)        0 2023-09-16 07:19:17.737105 ScrollableContainers-1.1.2/src/ScrollableContainers/
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)      697 2023-05-21 21:11:52.000000 ScrollableContainers-1.1.2/src/ScrollableContainers/Qt5.py
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)      711 2023-05-21 21:11:52.000000 ScrollableContainers-1.1.2/src/ScrollableContainers/Qt6.py
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)     6328 2023-09-16 07:17:47.000000 ScrollableContainers-1.1.2/src/ScrollableContainers/Tk.py
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)      635 2023-05-21 21:11:52.000000 ScrollableContainers-1.1.2/src/ScrollableContainers/Wx.py
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)      132 2023-09-16 07:17:47.000000 ScrollableContainers-1.1.2/src/ScrollableContainers/__init__.py
-drwxr-xr-x   0 tfpf      (1000) tfpf      (1000)        0 2023-09-16 07:19:17.737105 ScrollableContainers-1.1.2/src/ScrollableContainers.egg-info/
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)     4467 2023-09-16 07:19:17.000000 ScrollableContainers-1.1.2/src/ScrollableContainers.egg-info/PKG-INFO
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)      390 2023-09-16 07:19:17.000000 ScrollableContainers-1.1.2/src/ScrollableContainers.egg-info/SOURCES.txt
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)        1 2023-09-16 07:19:17.000000 ScrollableContainers-1.1.2/src/ScrollableContainers.egg-info/dependency_links.txt
--rw-r--r--   0 tfpf      (1000) tfpf      (1000)       21 2023-09-16 07:19:17.000000 ScrollableContainers-1.1.2/src/ScrollableContainers.egg-info/top_level.txt
+-rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/SECURITY.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.github/workflows/install.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/examples/README.md
+-rwxr-xr-x   0        0        0     1519 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/examples/examples_ScrollableAreaQt5.py
+-rwxr-xr-x   0        0        0     1519 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/examples/examples_ScrollableAreaQt6.py
+-rwxr-xr-x   0        0        0     1286 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/examples/examples_ScrollableFrameTk.py
+-rwxr-xr-x   0        0        0     1350 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/examples/examples_ScrollablePanelWx.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/src/ScrollableContainers/__init__.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/src/ScrollableContainers/_qt5.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/src/ScrollableContainers/_qt6.py
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/src/ScrollableContainers/_tk.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/src/ScrollableContainers/_wx.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.gitignore
+-rw-r--r--   0        0        0    31917 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/COPYING.md
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/README.md
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/PKG-INFO
```

### Comparing `ScrollableContainers-1.1.2/COPYING.md` & `scrollablecontainers-2.0.1a0/COPYING.md`

 * *Files identical despite different names*

### Comparing `ScrollableContainers-1.1.2/PKG-INFO` & `scrollablecontainers-2.0.1a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: ScrollableContainers
-Version: 1.1.2
-Summary: Scrollable containers for Tkinter, wxPython, PyQt5 and PyQt6
-Author: Vishal Pankaj Chandratreya
-Project-URL: Homepage, https://github.com/tfpf/ScrollableContainers
-Project-URL: Bug Tracker, https://github.com/tfpf/ScrollableContainers/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: COPYING.md
-
 # Scrollable containers which *just work*!
 If you have developed GUI applications, you probably know the pain of designing a clean front-end only to find that
 your application window is too large for your client's screen. Making the content scrollable is not straightforward (at
 least in Tkinter). Especially not after you have already written a lot of code to draw the content.
 
 You can use `ScrollableContainers` to reduce headaches.
 [It's available on PyPI!](https://pypi.org/project/ScrollableContainers/)
@@ -30,14 +16,18 @@
 * PyQt5
 * PyQt6
 
 **This project is not sponsored or endorsed by, or connected with, any organisation or entity such as but not limited
 to: the Tcl Core Team, the Python Software Foundation, the wxWidgets Team, the wxPython Team, the Qt Company and
 Riverbank Computing.**
 
+[![lint](https://github.com/tfpf/ScrollableContainers/actions/workflows/lint.yml/badge.svg)](https://github.com/tfpf/ScrollableContainers/actions/workflows/lint.yml)
+[![install](https://github.com/tfpf/ScrollableContainers/actions/workflows/install.yml/badge.svg)](https://github.com/tfpf/ScrollableContainers/actions/workflows/install.yml)
+[![build](https://github.com/tfpf/ScrollableContainers/actions/workflows/build.yml/badge.svg)](https://github.com/tfpf/ScrollableContainers/actions/workflows/build.yml)
+
 # Tkinter
 `ScrollableContainers.ScrollableFrameTk`: a comprehensive implementation of a scrollable frame, and the flagship class
 of this project. (I wrote the other classes just for completeness.)
 
 ### Usage
 Add widgets to the `frame` attribute of a `ScrollableFrameTk` object.
 [See examples.](https://github.com/tfpf/ScrollableContainers/blob/main/examples/examples_ScrollableFrameTk.py)
```

### Comparing `ScrollableContainers-1.1.2/README.md` & `scrollablecontainers-2.0.1a0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.3
+Name: ScrollableContainers
+Version: 2.0.1a0
+Summary: Scrollable containers for Tkinter, wxPython, PyQt5 and PyQt6
+Project-URL: Homepage, https://github.com/tfpf/ScrollableContainers
+Project-URL: Bug Tracker, https://github.com/tfpf/ScrollableContainers/issues
+Author: Vishal Pankaj Chandratreya
+License-File: COPYING.md
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Provides-Extra: qt5
+Requires-Dist: pyqt5; extra == 'qt5'
+Provides-Extra: qt6
+Requires-Dist: pyqt6; extra == 'qt6'
+Provides-Extra: wx
+Requires-Dist: wxpython; extra == 'wx'
+Description-Content-Type: text/markdown
+
 # Scrollable containers which *just work*!
 If you have developed GUI applications, you probably know the pain of designing a clean front-end only to find that
 your application window is too large for your client's screen. Making the content scrollable is not straightforward (at
 least in Tkinter). Especially not after you have already written a lot of code to draw the content.
 
 You can use `ScrollableContainers` to reduce headaches.
 [It's available on PyPI!](https://pypi.org/project/ScrollableContainers/)
@@ -16,14 +36,18 @@
 * PyQt5
 * PyQt6
 
 **This project is not sponsored or endorsed by, or connected with, any organisation or entity such as but not limited
 to: the Tcl Core Team, the Python Software Foundation, the wxWidgets Team, the wxPython Team, the Qt Company and
 Riverbank Computing.**
 
+[![lint](https://github.com/tfpf/ScrollableContainers/actions/workflows/lint.yml/badge.svg)](https://github.com/tfpf/ScrollableContainers/actions/workflows/lint.yml)
+[![install](https://github.com/tfpf/ScrollableContainers/actions/workflows/install.yml/badge.svg)](https://github.com/tfpf/ScrollableContainers/actions/workflows/install.yml)
+[![build](https://github.com/tfpf/ScrollableContainers/actions/workflows/build.yml/badge.svg)](https://github.com/tfpf/ScrollableContainers/actions/workflows/build.yml)
+
 # Tkinter
 `ScrollableContainers.ScrollableFrameTk`: a comprehensive implementation of a scrollable frame, and the flagship class
 of this project. (I wrote the other classes just for completeness.)
 
 ### Usage
 Add widgets to the `frame` attribute of a `ScrollableFrameTk` object.
 [See examples.](https://github.com/tfpf/ScrollableContainers/blob/main/examples/examples_ScrollableFrameTk.py)
```

### Comparing `ScrollableContainers-1.1.2/src/ScrollableContainers/Qt5.py` & `scrollablecontainers-2.0.1a0/src/ScrollableContainers/_qt5.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-__all__ = ['ScrollableAreaQt5']
+__all__ = ["ScrollableAreaQt5"]
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import QScrollArea, QVBoxLayout, QWidget
 
 
 class ScrollableAreaQt5(QScrollArea):
     """
-Container with horizontal and vertical scrolling capabilities. Widgets must be
-added to its `area` attribute.
+    Container with horizontal and vertical scrolling capabilities. Widgets must
+    be added to its `area` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # This object only allows a container to be placed in it.
         container = QWidget()
```

### Comparing `ScrollableContainers-1.1.2/src/ScrollableContainers/Qt6.py` & `scrollablecontainers-2.0.1a0/src/ScrollableContainers/_qt6.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-__all__ = ['ScrollableAreaQt6']
+__all__ = ["ScrollableAreaQt6"]
 
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import QScrollArea, QVBoxLayout, QWidget
 
 
 class ScrollableAreaQt6(QScrollArea):
     """
-Container with horizontal and vertical scrolling capabilities. Widgets must be
-added to its `area` attribute.
+    Container with horizontal and vertical scrolling capabilities. Widgets must
+    be added to its `area` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # This object only allows a container to be placed in it.
         container = QWidget()
```

### Comparing `ScrollableContainers-1.1.2/src/ScrollableContainers/Tk.py` & `scrollablecontainers-2.0.1a0/src/ScrollableContainers/_tk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,165 +1,166 @@
-__all__ = ['ScrollableFrameTk']
+__all__ = ["ScrollableFrameTk"]
 
 import platform
 import tkinter as tk
-import tkinter.ttk as ttk
+from tkinter import ttk
 
 _system = platform.system()
 
 
 class ScrollableFrameTk(ttk.Frame):
     """
-Container with horizontal and vertical scrolling capabilities. Widgets must be
-added to its `frame` attribute.
+    Container with horizontal and vertical scrolling capabilities. Widgets must
+    be added to its `frame` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Scrollable canvas. This is the widget which actually manages
         # scrolling. Using the grid geometry manager ensures that the
         # horizontal and vertical scrollbars do not meet.
         self._canvas = tk.Canvas(self)
-        self._canvas.bind('<Configure>', self._on_canvas_configure)
-        self._canvas.bind('<Enter>', self._on_canvas_enter)
-        self._canvas.bind('<Leave>', self._on_canvas_leave)
+        self._canvas.bind("<Configure>", self._on_canvas_configure)
+        self._canvas.bind("<Enter>", self._on_canvas_enter)
+        self._canvas.bind("<Leave>", self._on_canvas_leave)
         self._canvas.grid(row=0, column=0, sticky=tk.NSEW)
 
         xscrollbar = ttk.Scrollbar(self, orient=tk.HORIZONTAL, command=self._xview)
         xscrollbar.grid(row=1, column=0, sticky=tk.EW)
         yscrollbar = ttk.Scrollbar(self, orient=tk.VERTICAL, command=self._yview)
         yscrollbar.grid(row=0, column=1, sticky=tk.NS)
         self._canvas.configure(xscrollcommand=xscrollbar.set, yscrollcommand=yscrollbar.set)
 
         self.grid_rowconfigure(0, weight=1)
         self.grid_columnconfigure(0, weight=1)
 
         self.frame = ttk.Frame(self._canvas)
         self._window = self._canvas.create_window((0, 0), window=self.frame, anchor=tk.NW)
-        self.frame.bind('<Configure>', self._on_frame_configure)
-        self._on_frame_expose_id = self.frame.bind('<Expose>', self._on_frame_expose)
+        self.frame.bind("<Configure>", self._on_frame_configure)
+        self._on_frame_expose_id = self.frame.bind("<Expose>", self._on_frame_expose)
 
         # Initially, the vertical scrollbar is a hair below its topmost
         # position. Move it to said position. No harm in doing the equivalent
         # for the horizontal scrollbar.
         self._canvas.xview_moveto(0.0)
         self._canvas.yview_moveto(0.0)
 
     def _xview(self, *args, width=None):
         """
-Called when a horizontal scroll is requested. Called by some other callbacks
-(`_on_canvas_configure` and `_on_frame_configure`) whenever it is necessary to
-horizontally realign the contents of the canvas. Scroll the view only if the
-contents are not completely visible. Otherwise, move the scrollbar to such a
-position that they are horizontally centred.
+        Called when a horizontal scroll is requested. Called by other callbacks
+        (`_on_canvas_configure` and `_on_frame_configure`) whenever it is
+        necessary to horizontally realign the contents of the canvas. Scroll
+        the view only if the contents are not completely visible. Otherwise,
+        move the scrollbar to such a position that they are horizontally
+        centred.
 
-:param args: Tuple which can be passed to `tkinter.Canvas.xview`.
-:param width: Width of the canvas.
+        :param args: Tuple which can be passed to `tkinter.Canvas.xview`.
+        :param width: Width of the canvas.
         """
         if self._canvas.xview() != (0.0, 1.0):
             self._canvas.xview(*args)
         else:
             width = width or self._canvas.winfo_width()
 
             # To move the contents of the canvas to the centre, I call this
             # function with a negative argument. I don't know if this hack is
             # supported (because the Tcl/Tk manual pages say that it must be a
             # fraction between 0 and 1), but it works!
             self._canvas.xview_moveto((1 - width / self.frame.winfo_width()) / 2)
 
     def _yview(self, *args):
         """
-Called when a vertical scroll is requested. Scroll the view only if the
-contents are not completely visible.
+        Called when a vertical scroll is requested. Scroll the view only if the
+        contents are not completely visible.
 
-:param args: Tuple which can be passed to `tkinter.Canvas.yview`.
+        :param args: Tuple which can be passed to `tkinter.Canvas.yview`.
         """
         if self._canvas.yview() != (0.0, 1.0):
             self._canvas.yview(*args)
 
     def _on_canvas_configure(self, event):
         """
-Called when the canvas is resized. Update the scrollable region.
+        Called when the canvas is resized. Update the scrollable region.
 
-:param event: Configure event.
+        :param event: Configure event.
         """
         self._canvas.configure(scrollregion=self._canvas.bbox(tk.ALL))
         self._xview(tk.SCROLL, 0, tk.UNITS, width=event.width)
 
-    def _on_frame_configure(self, event=None):
+    def _on_frame_configure(self, _=None):
         """
-Called when the frame is resized or the canvas is scrolled. Update the
-scrollable region.
+        Called when the frame is resized or the canvas is scrolled. Update the
+        scrollable region.
 
-This method is necessary to handle updates which may occur after the GUI loop
-has started.
+        This method is necessary to handle updates which may occur after the
+        GUI loop has started.
 
-:param event: Configure event.
+        :param _: Configure event.
         """
         self._canvas.configure(scrollregion=self._canvas.bbox(tk.ALL))
         self._xview(tk.SCROLL, 0, tk.UNITS)
 
-    def _on_frame_expose(self, event=None):
+    def _on_frame_expose(self, _=None):
         """
-Called when the frame becomes visible. Call `_on_frame_configure` and then
-disable this callback.
+        Called when the frame becomes visible. Call `_on_frame_configure` and
+        then disable this callback.
 
-This method is necessary because if a scrollable frame is put into, say, a
-notebook (as opposed to a toplevel window), and the canvas is wider than its
-contents, then (on Linux) the contents are not initially horizontally centred.
-(This issue is not observed on Windows, probably because its frame configure
-events work differently.) Hence, I try to centre the contents again upon an
-expose event.
+        This method is necessary because if a scrollable frame is put into,
+        say, a notebook (as opposed to a toplevel window), and the canvas is
+        wider than its contents, then (on Linux) the contents are not initially
+        horizontally centred. (This issue is not observed on Windows, probably
+        because its frame configure events work differently.) Hence, I try to
+        centre the contents again upon an expose event.
 
-:param event: Expose event.
+        :param _: Expose event.
         """
         self._on_frame_configure()
-        self.frame.unbind('<Expose>', self._on_frame_expose_id)
+        self.frame.unbind("<Expose>", self._on_frame_expose_id)
 
-    def _on_canvas_enter(self, event=None):
+    def _on_canvas_enter(self, _=None):
         """
-Called when the mouse pointer enters the canvas. Set up vertical scrolling with
-the mouse wheel.
+        Called when the mouse pointer enters the canvas. Set up vertical
+        scrolling with the mouse wheel.
 
-:param event: Enter event.
+        :param _: Enter event.
         """
-        self.bind_all('<Button-4>', self._on_mouse_scroll)
-        self.bind_all('<Button-5>', self._on_mouse_scroll)
-        self.bind_all('<MouseWheel>', self._on_mouse_scroll)
+        self.bind_all("<Button-4>", self._on_mouse_scroll)
+        self.bind_all("<Button-5>", self._on_mouse_scroll)
+        self.bind_all("<MouseWheel>", self._on_mouse_scroll)
 
-    def _on_canvas_leave(self, event=None):
+    def _on_canvas_leave(self, _=None):
         """
-Called when the mouse pointer leaves the canvas. Unset vertical scrolling with
-the mouse wheel.
+        Called when the mouse pointer leaves the canvas. Unset vertical
+        scrolling with the mouse wheel.
 
-:param event: Leave event.
+        :param _: Leave event.
         """
-        self.unbind_all('<Button-4>')
-        self.unbind_all('<Button-5>')
-        self.unbind_all('<MouseWheel>')
+        self.unbind_all("<Button-4>")
+        self.unbind_all("<Button-5>")
+        self.unbind_all("<MouseWheel>")
 
     def _on_mouse_scroll(self, event):
         """
-Called when the mouse wheel is scrolled or a two-finger swipe gesture is
-performed on the touchpad. Ask to scroll the view horizontally if the mouse
-wheel is scrolled with Shift held down (equivalent to a horizontal two-finger
-swipe) and vertically otherwise (equivalent to a vertical two-finger swipe).
+        Called when the mouse wheel is scrolled or a two-finger swipe gesture
+        is performed on the touchpad. Ask to scroll the view horizontally if
+        the mouse wheel is scrolled with Shift held down (equivalent to a
+        horizontal two-finger swipe) and vertically otherwise (equivalent to a
+        vertical two-finger swipe).
 
-:param event: Scroll event.
+        :param event: Scroll event.
         """
         # Select which method to call based on whether Shift was held down.
         # This is indicated by the LSB of the state.
-        if event.state & 1:
-            callee = self._xview
-        else:
-            callee = self._yview
-
-        if _system == 'Linux':
-            if event.num == 4:
+        callee = self._xview if event.state & 1 else self._yview
+        match _system:
+            case "Linux" if event.num == 4:
                 callee(tk.SCROLL, -1, tk.UNITS)
-            elif event.num == 5:
+            case "Linux" if event.num == 5:
                 callee(tk.SCROLL, 1, tk.UNITS)
-        elif _system == 'Darwin':
-            callee(tk.SCROLL, -event.delta, tk.UNITS)
-        elif _system == 'Windows':
-            callee(tk.SCROLL, -event.delta // 120, tk.UNITS)
+            case "Darwin":
+                callee(tk.SCROLL, -event.delta, tk.UNITS)
+            case "Windows":
+                callee(tk.SCROLL, -event.delta // 120, tk.UNITS)
+            case _:
+                message = f"event {event.num} on OS {_system!r} is not supported"
+                raise ValueError(message)
```

### Comparing `ScrollableContainers-1.1.2/src/ScrollableContainers/Wx.py` & `scrollablecontainers-2.0.1a0/src/ScrollableContainers/_wx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-__all__ = ['ScrollablePanelWx']
+__all__ = ["ScrollablePanelWx"]
 
 import wx
-import wx.lib.scrolledpanel as scrolledpanel
+from wx.lib import scrolledpanel
 
 
 class ScrollablePanelWx(scrolledpanel.ScrolledPanel):
     """
-Container with horizontal and vertical scrolling capabilities. Widgets must be
-added to its `panel` attribute.
+    Container with horizontal and vertical scrolling capabilities. Widgets must
+    be added to its `panel` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # According to the documentation, a sizer is required to calculate the
         # minimum virtual size of the panel.
```

