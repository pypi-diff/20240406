# Comparing `tmp/qtlink-1.0.5.tar.gz` & `tmp/qtlink-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.0.5.tar", last modified: Fri Apr  5 07:07:36 2024, max compression
+gzip compressed data, was "qtlink-1.0.6.tar", last modified: Fri Apr  5 13:57:01 2024, max compression
```

## Comparing `qtlink-1.0.5.tar` & `qtlink-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 07:07:36.623731 qtlink-1.0.5/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      515 2024-04-05 07:07:36.619732 qtlink-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 07:07:36.492958 qtlink-1.0.5/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-04 02:24:16.000000 qtlink-1.0.5/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 07:07:36.546205 qtlink-1.0.5/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.0.5/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.0.5/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.0.5/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     1874 2024-04-03 12:51:18.000000 qtlink-1.0.5/qtlink/dialog/dialog_use_table.py
-drwxrwxrwx   0        0        0        0 2024-04-05 07:07:36.562727 qtlink-1.0.5/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.5/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     1887 2024-04-03 08:29:47.000000 qtlink-1.0.5/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-05 07:07:36.590732 qtlink-1.0.5/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.5/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     5621 2024-04-03 12:28:17.000000 qtlink-1.0.5/qtlink/table/multiple_select_table_controller.py
--rw-rw-rw-   0        0        0     2087 2024-04-05 07:06:48.000000 qtlink-1.0.5/qtlink/table/single_select_table_controller.py
--rw-rw-rw-   0        0        0     6187 2024-04-03 09:55:09.000000 qtlink-1.0.5/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     3645 2024-04-04 02:24:16.000000 qtlink-1.0.5/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-05 07:07:36.616729 qtlink-1.0.5/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.0.5/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.0.5/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.0.5/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-05 07:07:36.618735 qtlink-1.0.5/qtlink.egg-info/
--rw-rw-rw-   0        0        0      515 2024-04-05 07:07:36.000000 qtlink-1.0.5/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2024-04-05 07:07:36.000000 qtlink-1.0.5/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 07:07:36.000000 qtlink-1.0.5/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-05 07:07:36.000000 qtlink-1.0.5/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 07:07:36.000000 qtlink-1.0.5/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 07:07:36.623731 qtlink-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      660 2024-04-05 07:06:48.000000 qtlink-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.170937 qtlink-1.0.6/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-04-05 13:57:01.168908 qtlink-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.127369 qtlink-1.0.6/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-04 02:24:16.000000 qtlink-1.0.6/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.158759 qtlink-1.0.6/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.0.6/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.0.6/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.0.6/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     1874 2024-04-03 12:51:18.000000 qtlink-1.0.6/qtlink/dialog/dialog_use_table.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.159806 qtlink-1.0.6/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.6/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     1887 2024-04-03 08:29:47.000000 qtlink-1.0.6/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.164401 qtlink-1.0.6/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.6/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     5653 2024-04-05 13:55:23.000000 qtlink-1.0.6/qtlink/table/multiple_select_table_controller.py
+-rw-rw-rw-   0        0        0     2107 2024-04-05 13:55:23.000000 qtlink-1.0.6/qtlink/table/single_select_table_controller.py
+-rw-rw-rw-   0        0        0     6207 2024-04-05 13:55:23.000000 qtlink-1.0.6/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     3645 2024-04-04 02:24:16.000000 qtlink-1.0.6/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.166402 qtlink-1.0.6/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.0.6/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.0.6/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.0.6/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.167900 qtlink-1.0.6/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-04-05 13:57:01.000000 qtlink-1.0.6/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2024-04-05 13:57:01.000000 qtlink-1.0.6/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 13:57:01.000000 qtlink-1.0.6/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-05 13:57:01.000000 qtlink-1.0.6/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 13:57:01.000000 qtlink-1.0.6/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 13:57:01.170937 qtlink-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      660 2024-04-05 13:56:46.000000 qtlink-1.0.6/setup.py
```

### Comparing `qtlink-1.0.5/LICENSE` & `qtlink-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.5/PKG-INFO` & `qtlink-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.0.5
+Version: 1.0.6
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.0.5/qtlink/dialog/dialog_choice.py` & `qtlink-1.0.6/qtlink/dialog/dialog_choice.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.5/qtlink/dialog/dialog_info.py` & `qtlink-1.0.6/qtlink/dialog/dialog_info.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.5/qtlink/dialog/dialog_use_table.py` & `qtlink-1.0.6/qtlink/dialog/dialog_use_table.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.5/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.0.6/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.5/qtlink/table/multiple_select_table_controller.py` & `qtlink-1.0.6/qtlink/table/multiple_select_table_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             self.save_current_column_widths()
         self.first_load = False
 
         self.model.clear()
         self.raw_data = model_data
         self.always_checked_data = always_checked_data if always_checked_data else []
         for data in model_data:
-            items = [QStandardItem(str(data[column]) if data[column] else '')
+            items = [QStandardItem(str(data.get(column, None)) if data.get(column, None) is not None else '')
                      for column in self.table_columns
                      if column not in hide_columns]
             items[0].setCheckable(True)
             if data in self.always_checked_data:
                 items[0].setCheckState(Qt.Checked)
                 # 禁用交互
                 for item in items:
```

### Comparing `qtlink-1.0.5/qtlink/table/single_select_table_controller.py` & `qtlink-1.0.6/qtlink/table/single_select_table_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             # 保存当前列宽
             self.save_current_column_widths()
         self.first_load = False
 
         self.model.clear()
         self.raw_data = model_data
         for data in model_data:
-            items = [QStandardItem(str(data[column]) if data[column] is not None else '')
+            items = [QStandardItem(str(data.get(column, None)) if data.get(column, None) is not None else '')
                      for column in self.table_columns
                      if column not in hide_columns]
             items[0].setCheckable(True)
             self.model.appendRow(items)
         self.update_table_columns(self.table_columns)
         # 重新连接信号
         self.model.itemChanged.connect(self.on_item_changed)
```

### Comparing `qtlink-1.0.5/qtlink/table/table_controller.py` & `qtlink-1.0.6/qtlink/table/table_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             # 保存当前列宽
             self.save_current_column_widths()
         self.first_load = False
 
         self.model.clear()
         self.raw_data = model_data
         for data in model_data:
-            items = [QStandardItem(str(data[column]) if data[column] is not None else '')
+            items = [QStandardItem(str(data.get(column, None)) if data.get(column, None) is not None else '')
                      for column in self.table_columns
                      if column not in hide_columns]
             self.model.appendRow(items)
         self.update_table_columns(self.table_columns)
 
     def update_table_columns(self, table_columns: list[str]):
         self.table_columns = table_columns
```

### Comparing `qtlink-1.0.5/qtlink/util.py` & `qtlink-1.0.6/qtlink/util.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.5/qtlink/widgets/drop_widget.py` & `qtlink-1.0.6/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.5/qtlink/widgets/list_widget.py` & `qtlink-1.0.6/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.5/qtlink.egg-info/PKG-INFO` & `qtlink-1.0.6/qtlink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.0.5
+Version: 1.0.6
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.0.5/qtlink.egg-info/SOURCES.txt` & `qtlink-1.0.6/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.5/setup.py` & `qtlink-1.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.0.5",
+    version="1.0.6",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6', 'matplotlib', 'numpy'],
```

