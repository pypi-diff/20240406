# Comparing `tmp/qtlink-1.0.6.tar.gz` & `tmp/qtlink-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.0.6.tar", last modified: Fri Apr  5 13:57:01 2024, max compression
+gzip compressed data, was "qtlink-1.0.7.tar", last modified: Sat Apr  6 05:56:42 2024, max compression
```

## Comparing `qtlink-1.0.6.tar` & `qtlink-1.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.170937 qtlink-1.0.6/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      515 2024-04-05 13:57:01.168908 qtlink-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.127369 qtlink-1.0.6/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-04 02:24:16.000000 qtlink-1.0.6/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.158759 qtlink-1.0.6/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.0.6/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.0.6/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.0.6/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     1874 2024-04-03 12:51:18.000000 qtlink-1.0.6/qtlink/dialog/dialog_use_table.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.159806 qtlink-1.0.6/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.6/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     1887 2024-04-03 08:29:47.000000 qtlink-1.0.6/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.164401 qtlink-1.0.6/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.6/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     5653 2024-04-05 13:55:23.000000 qtlink-1.0.6/qtlink/table/multiple_select_table_controller.py
--rw-rw-rw-   0        0        0     2107 2024-04-05 13:55:23.000000 qtlink-1.0.6/qtlink/table/single_select_table_controller.py
--rw-rw-rw-   0        0        0     6207 2024-04-05 13:55:23.000000 qtlink-1.0.6/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     3645 2024-04-04 02:24:16.000000 qtlink-1.0.6/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.166402 qtlink-1.0.6/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.0.6/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.0.6/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.0.6/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.167900 qtlink-1.0.6/qtlink.egg-info/
--rw-rw-rw-   0        0        0      515 2024-04-05 13:57:01.000000 qtlink-1.0.6/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2024-04-05 13:57:01.000000 qtlink-1.0.6/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 13:57:01.000000 qtlink-1.0.6/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-05 13:57:01.000000 qtlink-1.0.6/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 13:57:01.000000 qtlink-1.0.6/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 13:57:01.170937 qtlink-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      660 2024-04-05 13:56:46.000000 qtlink-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 05:56:42.686320 qtlink-1.0.7/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-04-06 05:56:42.685322 qtlink-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 05:56:42.510969 qtlink-1.0.7/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-04 02:24:16.000000 qtlink-1.0.7/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 05:56:42.584121 qtlink-1.0.7/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.0.7/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.0.7/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.0.7/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     1874 2024-04-03 12:51:18.000000 qtlink-1.0.7/qtlink/dialog/dialog_use_table.py
+drwxrwxrwx   0        0        0        0 2024-04-06 05:56:42.598828 qtlink-1.0.7/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.7/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     2036 2024-04-06 05:56:20.000000 qtlink-1.0.7/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-06 05:56:42.654356 qtlink-1.0.7/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.7/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     5653 2024-04-05 13:55:23.000000 qtlink-1.0.7/qtlink/table/multiple_select_table_controller.py
+-rw-rw-rw-   0        0        0     2107 2024-04-05 13:55:23.000000 qtlink-1.0.7/qtlink/table/single_select_table_controller.py
+-rw-rw-rw-   0        0        0     6207 2024-04-05 13:55:23.000000 qtlink-1.0.7/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     3645 2024-04-04 02:24:16.000000 qtlink-1.0.7/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-06 05:56:42.682786 qtlink-1.0.7/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.0.7/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.0.7/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.0.7/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-06 05:56:42.684308 qtlink-1.0.7/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-04-06 05:56:42.000000 qtlink-1.0.7/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2024-04-06 05:56:42.000000 qtlink-1.0.7/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 05:56:42.000000 qtlink-1.0.7/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-06 05:56:42.000000 qtlink-1.0.7/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-06 05:56:42.000000 qtlink-1.0.7/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 05:56:42.686320 qtlink-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      660 2024-04-06 05:56:20.000000 qtlink-1.0.7/setup.py
```

### Comparing `qtlink-1.0.6/LICENSE` & `qtlink-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/PKG-INFO` & `qtlink-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.0.6
+Version: 1.0.7
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.0.6/qtlink/dialog/dialog_choice.py` & `qtlink-1.0.7/qtlink/dialog/dialog_choice.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/qtlink/dialog/dialog_info.py` & `qtlink-1.0.7/qtlink/dialog/dialog_info.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/qtlink/dialog/dialog_use_table.py` & `qtlink-1.0.7/qtlink/dialog/dialog_use_table.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.0.7/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,23 +12,26 @@
     def __init__(self, enable_toolbar: bool = True, parent=None):
         super(MplCanvas, self).__init__(parent)
 
         self.canvas = FigureCanvas(Figure(figsize=(5, 4), constrained_layout=True))
         self.ax = self.canvas.figure.subplots()
 
         self.vertical_layout = QVBoxLayout()
-        if enable_toolbar:
+        self.enable_toolbar = enable_toolbar
+        if self.enable_toolbar:
             self.toolbar = NavigationToolbar(self.canvas, self)
             self.vertical_layout.addWidget(self.toolbar)
         self.vertical_layout.addWidget(self.canvas)
         self.setLayout(self.vertical_layout)
 
     def clear_canvas(self):
         self.canvas.figure.clear()
         self.ax = self.canvas.figure.subplots()
+        if self.enable_toolbar:
+            self.toolbar = NavigationToolbar(self.canvas, self)
         self.canvas.draw_idle()
 
     def plot_lines(self, data: list[dict],
                    x_label: str = '',
                    y_label: str = '',
                    title: str = ''):
```

### Comparing `qtlink-1.0.6/qtlink/table/multiple_select_table_controller.py` & `qtlink-1.0.7/qtlink/table/multiple_select_table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/qtlink/table/single_select_table_controller.py` & `qtlink-1.0.7/qtlink/table/single_select_table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/qtlink/table/table_controller.py` & `qtlink-1.0.7/qtlink/table/table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/qtlink/util.py` & `qtlink-1.0.7/qtlink/util.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/qtlink/widgets/drop_widget.py` & `qtlink-1.0.7/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/qtlink/widgets/list_widget.py` & `qtlink-1.0.7/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/qtlink.egg-info/PKG-INFO` & `qtlink-1.0.7/qtlink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.0.6
+Version: 1.0.7
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.0.6/qtlink.egg-info/SOURCES.txt` & `qtlink-1.0.7/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.6/setup.py` & `qtlink-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.0.6",
+    version="1.0.7",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6', 'matplotlib', 'numpy'],
```

