# Comparing `tmp/textalloc-0.1.0.tar.gz` & `tmp/textalloc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textalloc-0.1.0.tar", last modified: Fri Apr  5 17:42:09 2024, max compression
+gzip compressed data, was "textalloc-0.1.1.tar", last modified: Sat Apr  6 15:46:30 2024, max compression
```

## Comparing `textalloc-0.1.0.tar` & `textalloc-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-05 17:42:08.994909 textalloc-0.1.0/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-0.1.0/LICENSE
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7971 2024-04-05 17:42:08.986910 textalloc-0.1.0/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7308 2024-04-05 16:57:31.000000 textalloc-0.1.0/README.md
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-04-05 17:42:00.000000 textalloc-0.1.0/pyproject.toml
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-04-05 17:42:08.995909 textalloc-0.1.0/setup.cfg
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-05 17:42:08.706912 textalloc-0.1.0/src/
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-05 17:42:08.830909 textalloc-0.1.0/src/textalloc/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    15463 2024-04-05 17:35:06.000000 textalloc-0.1.0/src/textalloc/__init__.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-0.1.0/src/textalloc/candidates.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9795 2024-04-05 17:35:17.000000 textalloc-0.1.0/src/textalloc/non_overlapping_boxes.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-0.1.0/src/textalloc/overlap_functions.py
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-05 17:42:08.975912 textalloc-0.1.0/src/textalloc.egg-info/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7971 2024-04-05 17:42:08.000000 textalloc-0.1.0/src/textalloc.egg-info/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-04-05 17:42:08.000000 textalloc-0.1.0/src/textalloc.egg-info/SOURCES.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-04-05 17:42:08.000000 textalloc-0.1.0/src/textalloc.egg-info/dependency_links.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-04-05 17:42:08.000000 textalloc-0.1.0/src/textalloc.egg-info/requires.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-04-05 17:42:08.000000 textalloc-0.1.0/src/textalloc.egg-info/top_level.txt
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-06 15:46:30.292714 textalloc-0.1.1/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-0.1.1/LICENSE
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8270 2024-04-06 15:46:30.282715 textalloc-0.1.1/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7607 2024-04-06 15:42:17.000000 textalloc-0.1.1/README.md
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-04-06 15:45:24.000000 textalloc-0.1.1/pyproject.toml
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-04-06 15:46:30.293716 textalloc-0.1.1/setup.cfg
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-06 15:46:29.985719 textalloc-0.1.1/src/
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-06 15:46:30.129719 textalloc-0.1.1/src/textalloc/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    16415 2024-04-06 15:42:38.000000 textalloc-0.1.1/src/textalloc/__init__.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-0.1.1/src/textalloc/candidates.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9795 2024-04-05 17:35:17.000000 textalloc-0.1.1/src/textalloc/non_overlapping_boxes.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-0.1.1/src/textalloc/overlap_functions.py
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-06 15:46:30.272716 textalloc-0.1.1/src/textalloc.egg-info/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8270 2024-04-06 15:46:29.000000 textalloc-0.1.1/src/textalloc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-04-06 15:46:29.000000 textalloc-0.1.1/src/textalloc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-04-06 15:46:29.000000 textalloc-0.1.1/src/textalloc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-04-06 15:46:29.000000 textalloc-0.1.1/src/textalloc.egg-info/requires.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-04-06 15:46:29.000000 textalloc-0.1.1/src/textalloc.egg-info/top_level.txt
```

### Comparing `textalloc-0.1.0/LICENSE` & `textalloc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.0/PKG-INFO` & `textalloc-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -88,15 +88,15 @@
     provide a scatterplot object (scatter_plot=ax.scatter(...))
     for more exact placement instead of x_scatter, y_scatter, scatter_sizes etc.. default None.
 text_scatter_sizes: (array-like), default None
     sizes of text scattered objects in plot list of 1d arrays/lists.
 textsize: (Union[int, List[int]]), default 10
     Size of text.
 margin: (float), default 0.0
-    Parameter for margins between objects.
+    Parameter for margins between objects. Recommendation: keep this lower than min_distance.
     Increase for larger margins to points and lines.
     Given in proportion of x-ax dimensions (0-1)
 min_distance: (float), default 0.015
     Parameter for min distance from textbox to
     its plotted position.
     Given in proportion of x-ax dimensions (0-1)
 max_distance: (float), default 0.2
@@ -124,14 +124,18 @@
     (south, north, east, west, northeast, northwest, southeast, southwest).
 x_logscale_base: (int), default None
     Base of x-axis log-scale, required if the scaling of the x-axis is "log"
 y_logscale_base: (int), default None
     Base of y-axis log-scale, required if the scaling of the y-axis is "log"
 avoid_label_lines_overlap: (bool), default False
     If set to True, avoids overlap for drawn lines to text labels.
+src_crs: (object), default None
+    Default crs of data, required when using transform in kwargs.
+    For example one can set src_crs=cartopy.crs.TransverseMercator() which is
+    default in matplotlib if using transform=cartopy.crs.PlateCarree().
 **kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
```

### Comparing `textalloc-0.1.0/README.md` & `textalloc-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     provide a scatterplot object (scatter_plot=ax.scatter(...))
     for more exact placement instead of x_scatter, y_scatter, scatter_sizes etc.. default None.
 text_scatter_sizes: (array-like), default None
     sizes of text scattered objects in plot list of 1d arrays/lists.
 textsize: (Union[int, List[int]]), default 10
     Size of text.
 margin: (float), default 0.0
-    Parameter for margins between objects.
+    Parameter for margins between objects. Recommendation: keep this lower than min_distance.
     Increase for larger margins to points and lines.
     Given in proportion of x-ax dimensions (0-1)
 min_distance: (float), default 0.015
     Parameter for min distance from textbox to
     its plotted position.
     Given in proportion of x-ax dimensions (0-1)
 max_distance: (float), default 0.2
@@ -106,14 +106,18 @@
     (south, north, east, west, northeast, northwest, southeast, southwest).
 x_logscale_base: (int), default None
     Base of x-axis log-scale, required if the scaling of the x-axis is "log"
 y_logscale_base: (int), default None
     Base of y-axis log-scale, required if the scaling of the y-axis is "log"
 avoid_label_lines_overlap: (bool), default False
     If set to True, avoids overlap for drawn lines to text labels.
+src_crs: (object), default None
+    Default crs of data, required when using transform in kwargs.
+    For example one can set src_crs=cartopy.crs.TransverseMercator() which is
+    default in matplotlib if using transform=cartopy.crs.PlateCarree().
 **kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
```

### Comparing `textalloc-0.1.0/pyproject.toml` & `textalloc-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textalloc"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Christoffer Kjellson", email="c.kjellson@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Efficient Text Allocation in matplotlib using NumPy Broadcasting"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `textalloc-0.1.0/src/textalloc/__init__.py` & `textalloc-0.1.1/src/textalloc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     linewidth: float = 1,
     textcolor: Union[str, List[str]] = "k",
     seed: int = 0,
     direction: str = None,
     x_logscale_base: float = None,
     y_logscale_base: float = None,
     avoid_label_lines_overlap: bool = False,
+    src_crs: object = None,
     **kwargs,
 ):
     """Main function of allocating text-boxes in matplotlib plot
 
     Args:
         fig (_type_): matplotlib figure used for rendering textbox-sizes.
         ax (_type_): matplotlib axes used for plotting.
@@ -73,20 +74,27 @@
         linewidth (float, optional): width of line. Defaults to 1.
         textcolor (Union[str, List[str]], optional): color code of the text. Defaults to "k".
         seed (int, optional): seeds order of text allocations. Defaults to 0.
         direction (str, optional): set preferred location of the boxes (south, north, east, west, northeast, northwest, southeast, southwest). Defaults to None.
         x_logscale_base (int, optional): base of x-axis log-scale, required if the scaling of the x-axis is "log".
         y_logscale_base (int, optional): base of y-axis log-scale, required if the scaling of the y-axis is "log".
         avoid_label_lines_overlap (bool, optional): If True, avoids overlap with lines drawn between text labels and locations. Defaults to False.
+        src_crs (object, optional): Default crs of data, required when using transform in kwargs. For example one can set src_crs=cartopy.crs.TransverseMercator() which is default in matplotlib if using transform=cartopy.crs.PlateCarree(). Defaults to None.
         **kwargs (): kwargs for the plt.text() call.
     """
     t0 = time.time()
     aspect_ratio = fig.get_size_inches()[0] / fig.get_size_inches()[1]
+    aspect_ratio2 = ax.get_aspect()
     xlims = ax.get_xlim()
     ylims = ax.get_ylim()
+    if kwargs.get("transform", None) is not None:
+        assert src_crs is not None
+        extent = ax.get_extent(crs=kwargs.get("transform", None))
+        xlims = (extent[0], extent[1])
+        ylims = (extent[2], extent[3])
 
     # Ensure good inputs
     assert len(x) == len(y)
     x = np.array(x)
     y = np.array(y)
     if scatter_sizes is not None:
         scatter_sizes = np.array(scatter_sizes)
@@ -155,14 +163,20 @@
         zip(x, y, text_list, textsize), disable=not verbose
     ):
         ann = ax.text(x_coord, y_coord, s, size=ts)
         box = ax.transData.inverted().transform(
             ann.get_tightbbox(fig.canvas.get_renderer())
         )
         w, h = box[1][0] - box[0][0], box[1][1] - box[0][1]
+        # If aspect ratio has been set, the width and height needs to be compensated here.
+        if aspect_ratio2 != "auto":
+            w = w / (aspect_ratio2 / aspect_ratio)
+            h = h * (aspect_ratio2 / aspect_ratio)
+        if kwargs.get("transform", None) is not None:
+            w, h = kwargs.get("transform", None).transform_point(w, h, src_crs=src_crs)
         original_boxes.append((x_coord, y_coord, w, h, s))
         ann.remove()
 
     # If scatterplot exists, get scatter bboxes
     scatter_plot_bbs = None
     if scatter_plot is not None:
         scatter_plot_bbs = get_scatter_bbs(scatter_plot, ax)
@@ -307,14 +321,15 @@
             )
             if x_near is not None:
                 ax.plot(
                     [x[ind], x_near],
                     [y[ind], y_near],
                     linewidth=linewidth,
                     c=linecolor[ind],
+                    **kwargs,
                 )
     for x_coord, y_coord, w, h, s, ind in non_overlapping_boxes:
         ax.text(x_coord, y_coord, s, size=textsize[ind], c=textcolor[ind], **kwargs)
 
     if draw_all:
         for ind in overlapping_boxes_inds:
             ax.text(
```

### Comparing `textalloc-0.1.0/src/textalloc/candidates.py` & `textalloc-0.1.1/src/textalloc/candidates.py`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.0/src/textalloc/non_overlapping_boxes.py` & `textalloc-0.1.1/src/textalloc/non_overlapping_boxes.py`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.0/src/textalloc/overlap_functions.py` & `textalloc-0.1.1/src/textalloc/overlap_functions.py`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.0/src/textalloc.egg-info/PKG-INFO` & `textalloc-0.1.1/src/textalloc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -88,15 +88,15 @@
     provide a scatterplot object (scatter_plot=ax.scatter(...))
     for more exact placement instead of x_scatter, y_scatter, scatter_sizes etc.. default None.
 text_scatter_sizes: (array-like), default None
     sizes of text scattered objects in plot list of 1d arrays/lists.
 textsize: (Union[int, List[int]]), default 10
     Size of text.
 margin: (float), default 0.0
-    Parameter for margins between objects.
+    Parameter for margins between objects. Recommendation: keep this lower than min_distance.
     Increase for larger margins to points and lines.
     Given in proportion of x-ax dimensions (0-1)
 min_distance: (float), default 0.015
     Parameter for min distance from textbox to
     its plotted position.
     Given in proportion of x-ax dimensions (0-1)
 max_distance: (float), default 0.2
@@ -124,14 +124,18 @@
     (south, north, east, west, northeast, northwest, southeast, southwest).
 x_logscale_base: (int), default None
     Base of x-axis log-scale, required if the scaling of the x-axis is "log"
 y_logscale_base: (int), default None
     Base of y-axis log-scale, required if the scaling of the y-axis is "log"
 avoid_label_lines_overlap: (bool), default False
     If set to True, avoids overlap for drawn lines to text labels.
+src_crs: (object), default None
+    Default crs of data, required when using transform in kwargs.
+    For example one can set src_crs=cartopy.crs.TransverseMercator() which is
+    default in matplotlib if using transform=cartopy.crs.PlateCarree().
 **kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
```

