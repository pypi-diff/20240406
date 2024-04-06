# Comparing `tmp/Comel-0.2.2.tar.gz` & `tmp/Comel-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Comel-0.2.2.tar", last modified: Sun Mar 31 08:14:14 2024, max compression
+gzip compressed data, was "Comel-0.2.3.tar", last modified: Sat Apr  6 09:11:26 2024, max compression
```

## Comparing `Comel-0.2.2.tar` & `Comel-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 08:14:14.778140 Comel-0.2.2/
-drwxrwxrwx   0        0        0        0 2024-03-31 08:14:14.776140 Comel-0.2.2/Comel.egg-info/
--rw-rw-rw-   0        0        0     5637 2024-03-31 08:14:14.000000 Comel-0.2.2/Comel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2024-03-31 08:14:14.000000 Comel-0.2.2/Comel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 08:14:14.000000 Comel-0.2.2/Comel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-03-31 08:14:14.000000 Comel-0.2.2/Comel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-31 08:14:14.000000 Comel-0.2.2/Comel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2022-11-18 08:59:38.000000 Comel-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       55 2023-10-28 23:55:47.000000 Comel-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5637 2024-03-31 08:14:14.777140 Comel-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3260 2023-10-28 23:55:47.000000 Comel-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 08:14:14.763380 Comel-0.2.2/comel/
--rw-rw-rw-   0        0        0      197 2024-03-31 08:13:15.000000 Comel-0.2.2/comel/__init__.py
--rw-rw-rw-   0        0        0       35 2023-10-26 13:51:01.000000 Comel-0.2.2/comel/constants.py
-drwxrwxrwx   0        0        0        0 2024-03-31 08:14:14.775141 Comel-0.2.2/comel/icons/
--rw-rw-rw-   0        0        0      334 2024-03-31 07:32:15.000000 Comel-0.2.2/comel/icons/branch-closed.png
--rw-rw-rw-   0        0        0      182 2024-03-31 07:32:13.000000 Comel-0.2.2/comel/icons/branch-end.png
--rw-rw-rw-   0        0        0      136 2024-03-31 07:32:11.000000 Comel-0.2.2/comel/icons/branch-more.png
--rw-rw-rw-   0        0        0      346 2024-03-31 07:32:17.000000 Comel-0.2.2/comel/icons/branch-open.png
--rw-rw-rw-   0        0        0      698 2023-10-28 23:55:47.000000 Comel-0.2.2/comel/icons/checked-disabled.png
--rw-rw-rw-   0        0        0      578 2023-10-28 23:55:47.000000 Comel-0.2.2/comel/icons/checked.png
--rw-rw-rw-   0        0        0     2916 2024-03-31 07:51:14.000000 Comel-0.2.2/comel/icons/dark-branch-closed.png
--rw-rw-rw-   0        0        0     2932 2024-03-31 07:50:38.000000 Comel-0.2.2/comel/icons/dark-branch-end.png
--rw-rw-rw-   0        0        0     2840 2024-03-31 07:50:31.000000 Comel-0.2.2/comel/icons/dark-branch-more.png
--rw-rw-rw-   0        0        0     2912 2024-03-31 07:51:12.000000 Comel-0.2.2/comel/icons/dark-branch-open.png
--rw-rw-rw-   0        0        0      698 2023-10-28 23:55:47.000000 Comel-0.2.2/comel/icons/dark-checked-disabled.png
--rw-rw-rw-   0        0        0      698 2023-10-28 23:55:47.000000 Comel-0.2.2/comel/icons/dark-checked.png
--rw-rw-rw-   0        0        0      881 2023-10-28 23:55:47.000000 Comel-0.2.2/comel/icons/dark-radio-off.png
--rw-rw-rw-   0        0        0     1107 2023-10-28 23:55:47.000000 Comel-0.2.2/comel/icons/dark-radio-on.png
--rw-rw-rw-   0        0        0     2904 2024-03-31 07:50:34.000000 Comel-0.2.2/comel/icons/dark-vline.png
--rw-rw-rw-   0        0        0     1007 2023-10-28 23:55:47.000000 Comel-0.2.2/comel/icons/radio-off.png
--rw-rw-rw-   0        0        0     1275 2023-10-28 23:55:47.000000 Comel-0.2.2/comel/icons/radio-on.png
--rw-rw-rw-   0        0        0      124 2024-03-31 07:32:08.000000 Comel-0.2.2/comel/icons/vline.png
-drwxrwxrwx   0        0        0        0 2024-03-31 08:14:14.776140 Comel-0.2.2/comel/themes/
--rw-rw-rw-   0        0        0     7669 2024-03-31 08:07:59.000000 Comel-0.2.2/comel/themes/dark.qss
--rw-rw-rw-   0        0        0     7658 2024-03-31 08:07:59.000000 Comel-0.2.2/comel/themes/light.qss
--rw-rw-rw-   0        0        0     1150 2023-10-28 23:55:47.000000 Comel-0.2.2/comel/widgets.py
--rw-rw-rw-   0        0        0     1213 2023-10-28 23:55:47.000000 Comel-0.2.2/comel/wrapper.py
--rw-rw-rw-   0        0        0     1422 2023-10-03 15:35:02.000000 Comel-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       21 2023-10-03 14:05:16.000000 Comel-0.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 08:14:14.778140 Comel-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-10-03 15:35:02.000000 Comel-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:11:26.188325 Comel-0.2.3/
+drwxrwxrwx   0        0        0        0 2024-04-06 09:11:26.187325 Comel-0.2.3/Comel.egg-info/
+-rw-rw-rw-   0        0        0     5637 2024-04-06 09:11:26.000000 Comel-0.2.3/Comel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2024-04-06 09:11:26.000000 Comel-0.2.3/Comel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 09:11:26.000000 Comel-0.2.3/Comel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-06 09:11:26.000000 Comel-0.2.3/Comel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-06 09:11:26.000000 Comel-0.2.3/Comel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2022-11-18 08:59:38.000000 Comel-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-10-28 23:55:47.000000 Comel-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5637 2024-04-06 09:11:26.188325 Comel-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3260 2023-10-28 23:55:47.000000 Comel-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 09:11:26.161978 Comel-0.2.3/comel/
+-rw-rw-rw-   0        0        0      197 2024-04-06 09:08:54.000000 Comel-0.2.3/comel/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-10-26 13:51:01.000000 Comel-0.2.3/comel/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:11:26.185328 Comel-0.2.3/comel/icons/
+-rw-rw-rw-   0        0        0      334 2024-03-31 07:32:15.000000 Comel-0.2.3/comel/icons/branch-closed.png
+-rw-rw-rw-   0        0        0      182 2024-03-31 07:32:13.000000 Comel-0.2.3/comel/icons/branch-end.png
+-rw-rw-rw-   0        0        0      136 2024-03-31 07:32:11.000000 Comel-0.2.3/comel/icons/branch-more.png
+-rw-rw-rw-   0        0        0      346 2024-03-31 07:32:17.000000 Comel-0.2.3/comel/icons/branch-open.png
+-rw-rw-rw-   0        0        0      698 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/checked-disabled.png
+-rw-rw-rw-   0        0        0      578 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/checked.png
+-rw-rw-rw-   0        0        0     2916 2024-03-31 07:51:14.000000 Comel-0.2.3/comel/icons/dark-branch-closed.png
+-rw-rw-rw-   0        0        0     2932 2024-03-31 07:50:38.000000 Comel-0.2.3/comel/icons/dark-branch-end.png
+-rw-rw-rw-   0        0        0     2840 2024-03-31 07:50:31.000000 Comel-0.2.3/comel/icons/dark-branch-more.png
+-rw-rw-rw-   0        0        0     2912 2024-03-31 07:51:12.000000 Comel-0.2.3/comel/icons/dark-branch-open.png
+-rw-rw-rw-   0        0        0      698 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/dark-checked-disabled.png
+-rw-rw-rw-   0        0        0      698 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/dark-checked.png
+-rw-rw-rw-   0        0        0      881 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/dark-radio-off.png
+-rw-rw-rw-   0        0        0     1107 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/dark-radio-on.png
+-rw-rw-rw-   0        0        0     2904 2024-03-31 07:50:34.000000 Comel-0.2.3/comel/icons/dark-vline.png
+-rw-rw-rw-   0        0        0     1007 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/radio-off.png
+-rw-rw-rw-   0        0        0     1275 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/radio-on.png
+-rw-rw-rw-   0        0        0      124 2024-03-31 07:32:08.000000 Comel-0.2.3/comel/icons/vline.png
+drwxrwxrwx   0        0        0        0 2024-04-06 09:11:26.187325 Comel-0.2.3/comel/themes/
+-rw-rw-rw-   0        0        0     7932 2024-04-06 09:07:05.000000 Comel-0.2.3/comel/themes/dark.qss
+-rw-rw-rw-   0        0        0     7914 2024-04-06 09:07:05.000000 Comel-0.2.3/comel/themes/light.qss
+-rw-rw-rw-   0        0        0     1150 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/widgets.py
+-rw-rw-rw-   0        0        0     1213 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/wrapper.py
+-rw-rw-rw-   0        0        0     1422 2023-10-03 15:35:02.000000 Comel-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       21 2023-10-03 14:05:16.000000 Comel-0.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 09:11:26.188325 Comel-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-10-03 15:35:02.000000 Comel-0.2.3/setup.py
```

### Comparing `Comel-0.2.2/Comel.egg-info/PKG-INFO` & `Comel-0.2.3/Comel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Comel
-Version: 0.2.2
+Version: 0.2.3
 Summary: Opinionated PySide6 Light/Dark Theme Toggler.
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Huey Yeng
```

### Comparing `Comel-0.2.2/Comel.egg-info/SOURCES.txt` & `Comel-0.2.3/Comel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/LICENSE` & `Comel-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/PKG-INFO` & `Comel-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Comel
-Version: 0.2.2
+Version: 0.2.3
 Summary: Opinionated PySide6 Light/Dark Theme Toggler.
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Huey Yeng
```

### Comparing `Comel-0.2.2/README.md` & `Comel-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/checked-disabled.png` & `Comel-0.2.3/comel/icons/checked-disabled.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/checked.png` & `Comel-0.2.3/comel/icons/checked.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/dark-branch-closed.png` & `Comel-0.2.3/comel/icons/dark-branch-closed.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/dark-branch-end.png` & `Comel-0.2.3/comel/icons/dark-branch-end.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/dark-branch-more.png` & `Comel-0.2.3/comel/icons/dark-branch-more.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/dark-branch-open.png` & `Comel-0.2.3/comel/icons/dark-branch-open.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/dark-checked-disabled.png` & `Comel-0.2.3/comel/icons/dark-checked-disabled.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/dark-checked.png` & `Comel-0.2.3/comel/icons/dark-checked.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/dark-radio-off.png` & `Comel-0.2.3/comel/icons/dark-radio-off.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/dark-radio-on.png` & `Comel-0.2.3/comel/icons/dark-radio-on.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/dark-vline.png` & `Comel-0.2.3/comel/icons/dark-vline.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/radio-off.png` & `Comel-0.2.3/comel/icons/radio-off.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/icons/radio-on.png` & `Comel-0.2.3/comel/icons/radio-on.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/themes/dark.qss` & `Comel-0.2.3/comel/themes/dark.qss`

 * *Files 2% similar despite different names*

```diff
@@ -385,7 +385,21 @@
 QScrollBar::add-page, QScrollBar::sub-page {
   background: transparent;
 }
 
 QAbstractScrollArea::corner {
   background: transparent;
 }
+
+QDateEdit {
+  border-width: 1px;
+  border-style: solid;
+  background-color: rgb(85, 90, 95);
+}
+
+QCalendarWidget QWidget {
+  alternate-background-color: rgb(65, 70, 80);
+}
+
+QCalendarWidget QAbstractItemView:disabled {
+  color: rgb(128, 128, 128);
+}
```

### Comparing `Comel-0.2.2/comel/themes/light.qss` & `Comel-0.2.3/comel/themes/light.qss`

 * *Files 2% similar despite different names*

```diff
@@ -385,7 +385,21 @@
 QScrollBar::add-page, QScrollBar::sub-page {
   background: transparent;
 }
 
 QAbstractScrollArea::corner {
   background: transparent;
 }
+
+QDateEdit {
+  border-width: 1px;
+  border-style: solid;
+  background-color: white;
+}
+
+QCalendarWidget QWidget {
+  alternate-background-color: rgb(235, 235, 240);
+}
+
+QCalendarWidget QAbstractItemView:disabled {
+  color: rgb(184, 184, 184);
+}
```

### Comparing `Comel-0.2.2/comel/widgets.py` & `Comel-0.2.3/comel/widgets.py`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/comel/wrapper.py` & `Comel-0.2.3/comel/wrapper.py`

 * *Files identical despite different names*

### Comparing `Comel-0.2.2/pyproject.toml` & `Comel-0.2.3/pyproject.toml`

 * *Files identical despite different names*

