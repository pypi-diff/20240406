# Comparing `tmp/ctkdlib-4.0.tar.gz` & `tmp/ctkdlib-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctkdlib-4.0.tar", last modified: Wed Mar 13 10:59:43 2024, max compression
+gzip compressed data, was "ctkdlib-4.1.tar", last modified: Sat Apr  6 17:07:57 2024, max compression
```

## Comparing `ctkdlib-4.0.tar` & `ctkdlib-4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 10:59:43.311097 ctkdlib-4.0/
--rw-rw-rw-   0        0        0     1086 2024-01-18 07:56:50.000000 ctkdlib-4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1086 2024-03-13 10:59:43.311097 ctkdlib-4.0/PKG-INFO
--rw-rw-rw-   0        0        0      510 2024-03-13 10:43:59.000000 ctkdlib-4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-13 10:59:43.251276 ctkdlib-4.0/ctkdlib/
--rw-rw-rw-   0        0        0      685 2024-03-13 10:48:58.000000 ctkdlib-4.0/ctkdlib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 10:59:43.311097 ctkdlib-4.0/ctkdlib/custom_widgets/
--rw-rw-rw-   0        0        0      477 2024-03-12 10:56:48.000000 ctkdlib-4.0/ctkdlib/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 ctkdlib-4.0/ctkdlib/custom_widgets/color_wheel.png
--rw-rw-rw-   0        0        0    12066 2024-02-22 07:44:24.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_calendar.py
--rw-rw-rw-   0        0        0     8619 2024-02-22 07:43:03.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_chart.py
--rw-rw-rw-   0        0        0     7504 2024-02-12 11:58:17.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_colorpicker.py
--rw-rw-rw-   0        0        0     7855 2024-03-13 09:07:44.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_draw.py
--rw-rw-rw-   0        0        0     4391 2024-03-10 14:04:27.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_gif.py
--rw-rw-rw-   0        0        0     6822 2024-02-09 06:29:39.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_graph.py
--rw-rw-rw-   0        0        0     2282 2024-02-09 06:50:34.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_hyperlink.py
--rw-rw-rw-   0        0        0     8508 2024-03-12 13:28:00.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_meter.py
--rw-rw-rw-   0        0        0     5287 2024-03-12 14:02:06.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_popupmenu.py
--rw-rw-rw-   0        0        0    59314 2024-02-08 18:29:38.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_rangeslider.py
--rw-rw-rw-   0        0        0    11004 2024-03-12 12:30:12.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_spinbox.py
--rw-rw-rw-   0        0        0     3404 2024-03-13 09:04:59.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_tooltip.py
--rw-rw-rw-   0        0        0    18678 2024-03-13 10:52:17.000000 ctkdlib-4.0/ctkdlib/custom_widgets/ctk_video.py
--rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 ctkdlib-4.0/ctkdlib/custom_widgets/target.png
-drwxrwxrwx   0        0        0        0 2024-03-13 10:59:43.311097 ctkdlib-4.0/ctkdlib.egg-info/
--rw-rw-rw-   0        0        0     1086 2024-03-13 10:59:43.000000 ctkdlib-4.0/ctkdlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      814 2024-03-13 10:59:43.000000 ctkdlib-4.0/ctkdlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2024-03-13 10:59:43.000000 ctkdlib-4.0/ctkdlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-03-13 10:59:43.000000 ctkdlib-4.0/ctkdlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-13 10:59:43.000000 ctkdlib-4.0/ctkdlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      563 2024-03-13 10:59:43.321368 ctkdlib-4.0/setup.cfg
--rw-rw-rw-   0        0        0     1134 2024-03-13 10:50:17.000000 ctkdlib-4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:07:57.801661 ctkdlib-4.1/
+-rw-rw-rw-   0        0        0     1086 2024-01-18 07:56:50.000000 ctkdlib-4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1086 2024-04-06 17:07:57.801661 ctkdlib-4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2024-03-13 10:43:59.000000 ctkdlib-4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 17:07:57.144357 ctkdlib-4.1/ctkdlib/
+-rw-rw-rw-   0        0        0      685 2024-03-13 10:48:58.000000 ctkdlib-4.1/ctkdlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:07:57.801661 ctkdlib-4.1/ctkdlib/custom_widgets/
+-rw-rw-rw-   0        0        0      477 2024-03-12 10:56:48.000000 ctkdlib-4.1/ctkdlib/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 ctkdlib-4.1/ctkdlib/custom_widgets/color_wheel.png
+-rw-rw-rw-   0        0        0    12066 2024-02-22 07:44:24.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_calendar.py
+-rw-rw-rw-   0        0        0     8619 2024-02-22 07:43:03.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_chart.py
+-rw-rw-rw-   0        0        0     7504 2024-02-12 11:58:17.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_colorpicker.py
+-rw-rw-rw-   0        0        0     7849 2024-04-06 17:05:56.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_draw.py
+-rw-rw-rw-   0        0        0     4391 2024-03-10 14:04:27.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_gif.py
+-rw-rw-rw-   0        0        0     6822 2024-02-09 06:29:39.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_graph.py
+-rw-rw-rw-   0        0        0     2282 2024-02-09 06:50:34.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_hyperlink.py
+-rw-rw-rw-   0        0        0     8508 2024-03-12 13:28:00.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_meter.py
+-rw-rw-rw-   0        0        0     5287 2024-03-12 14:02:06.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_popupmenu.py
+-rw-rw-rw-   0        0        0    59314 2024-02-08 18:29:38.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_rangeslider.py
+-rw-rw-rw-   0        0        0    11004 2024-03-12 12:30:12.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_spinbox.py
+-rw-rw-rw-   0        0        0     3404 2024-03-13 09:04:59.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_tooltip.py
+-rw-rw-rw-   0        0        0    18678 2024-03-13 10:52:17.000000 ctkdlib-4.1/ctkdlib/custom_widgets/ctk_video.py
+-rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 ctkdlib-4.1/ctkdlib/custom_widgets/target.png
+drwxrwxrwx   0        0        0        0 2024-04-06 17:07:57.801661 ctkdlib-4.1/ctkdlib.egg-info/
+-rw-rw-rw-   0        0        0     1086 2024-04-06 17:07:56.000000 ctkdlib-4.1/ctkdlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      814 2024-04-06 17:07:57.000000 ctkdlib-4.1/ctkdlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2024-04-06 17:07:56.000000 ctkdlib-4.1/ctkdlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-06 17:07:56.000000 ctkdlib-4.1/ctkdlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-06 17:07:56.000000 ctkdlib-4.1/ctkdlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      563 2024-04-06 17:07:57.817289 ctkdlib-4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1134 2024-04-06 17:06:29.000000 ctkdlib-4.1/setup.py
```

### Comparing `ctkdlib-4.0/LICENSE.txt` & `ctkdlib-4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/PKG-INFO` & `ctkdlib-4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctkdlib
-Version: 4.0
+Version: 4.1
 Summary: A special widget library for CTkDesigner
 Home-page: https://github.com/Akascape/CTkDesigner
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,ctkdesigner,gui-builder,ui-designer,python-gui-builder
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ctkdlib-4.0/ctkdlib/__init__.py` & `ctkdlib-4.1/ctkdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/color_wheel.png` & `ctkdlib-4.1/ctkdlib/custom_widgets/color_wheel.png`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_calendar.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_calendar.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_chart.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_chart.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_colorpicker.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_colorpicker.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_draw.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.update()
         
         super().configure(image=self.ctk_image)
     
     def round_corners(self, img, radius):
         circle = Image.new('L', (radius * 2, radius * 2), 0)
         draw = ImageDraw.Draw(circle)
-        draw.ellipse((0, 0, radius * 2 - 1, radius * 2 - 1), fill=255)
+        draw.ellipse((0, 0, radius * 2 , radius * 2 ), fill=255)
         alpha = Image.new('L', (200,200), 255)
         w, h = (200,200)
         alpha.paste(circle.crop((0, 0, radius, radius)), (0, 0))
         alpha.paste(circle.crop((0, radius, radius, radius * 2)), (0, h - radius))
         alpha.paste(circle.crop((radius, 0, radius * 2, radius)), (w - radius, 0))
         alpha.paste(circle.crop((radius, radius, radius * 2, radius * 2)), (w - radius, h - radius))
         alpha = alpha.resize(img.size, resample=3).filter(ImageFilter.EDGE_ENHANCE_MORE).filter(ImageFilter.SMOOTH_MORE)
```

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_gif.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_gif.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_graph.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_graph.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_hyperlink.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_hyperlink.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_meter.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_meter.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_popupmenu.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_popupmenu.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_rangeslider.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_rangeslider.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_spinbox.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_spinbox.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_tooltip.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/ctk_video.py` & `ctkdlib-4.1/ctkdlib/custom_widgets/ctk_video.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib/custom_widgets/target.png` & `ctkdlib-4.1/ctkdlib/custom_widgets/target.png`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/ctkdlib.egg-info/PKG-INFO` & `ctkdlib-4.1/ctkdlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctkdlib
-Version: 4.0
+Version: 4.1
 Summary: A special widget library for CTkDesigner
 Home-page: https://github.com/Akascape/CTkDesigner
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,ctkdesigner,gui-builder,ui-designer,python-gui-builder
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ctkdlib-4.0/ctkdlib.egg-info/SOURCES.txt` & `ctkdlib-4.1/ctkdlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.0/setup.cfg` & `ctkdlib-4.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 746b 646c 6962 0d0a 7665 7273   = ctkdlib..vers
-00000020: 696f 6e20 3d20 342e 300d 0a64 6573 6372  ion = 4.0..descr
+00000020: 696f 6e20 3d20 342e 310d 0a64 6573 6372  ion = 4.1..descr
 00000030: 6970 7469 6f6e 203d 2041 2073 7065 6369  iption = A speci
 00000040: 616c 2077 6964 6765 7420 6c69 6272 6172  al widget librar
 00000050: 7920 666f 7220 4354 6b44 6573 6967 6e65  y for CTkDesigne
 00000060: 720d 0a6c 6f6e 675f 6465 7363 7269 7074  r..long_descript
 00000070: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
 00000080: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
 00000090: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
```

### Comparing `ctkdlib-4.0/setup.py` & `ctkdlib-4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'ctkdlib',
-    version = '4.0',
+    version = '4.1',
     description = "A special widget library for CTkDesigner",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkDesigner",
```

