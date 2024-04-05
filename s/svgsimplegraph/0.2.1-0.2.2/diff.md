# Comparing `tmp/svgsimplegraph-0.2.1.tar.gz` & `tmp/svgsimplegraph-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgsimplegraph-0.2.1.tar", last modified: Wed Mar 27 22:54:27 2024, max compression
+gzip compressed data, was "svgsimplegraph-0.2.2.tar", last modified: Fri Apr  5 23:33:34 2024, max compression
```

## Comparing `svgsimplegraph-0.2.1.tar` & `svgsimplegraph-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-03-27 22:54:27.736528 svgsimplegraph-0.2.1/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1072 2023-05-30 04:47:02.000000 svgsimplegraph-0.2.1/LICENSE
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-03-27 22:54:27.736289 svgsimplegraph-0.2.1/PKG-INFO
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     6599 2024-02-12 21:11:46.000000 svgsimplegraph-0.2.1/README.md
--rw-r--r--   0 garrettpetersen   (501) staff       (20)       38 2024-03-27 22:54:27.736606 svgsimplegraph-0.2.1/setup.cfg
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      957 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.1/setup.py
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-03-27 22:54:27.731234 svgsimplegraph-0.2.1/svgsimplegraph/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      124 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.1/svgsimplegraph/__init__.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    10527 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.1/svgsimplegraph/base.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    16487 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.1/svgsimplegraph/bubble_and_arrow.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    41504 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.1/svgsimplegraph/categorical.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    15007 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.1/svgsimplegraph/ribbon.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    10208 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.1/svgsimplegraph/utils.py
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-03-27 22:54:27.732717 svgsimplegraph-0.2.1/svgsimplegraph.egg-info/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-03-27 22:54:27.000000 svgsimplegraph-0.2.1/svgsimplegraph.egg-info/PKG-INFO
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      524 2024-03-27 22:54:27.000000 svgsimplegraph-0.2.1/svgsimplegraph.egg-info/SOURCES.txt
--rw-r--r--   0 garrettpetersen   (501) staff       (20)        1 2024-03-27 22:54:27.000000 svgsimplegraph-0.2.1/svgsimplegraph.egg-info/dependency_links.txt
--rw-r--r--   0 garrettpetersen   (501) staff       (20)       17 2024-03-27 22:54:27.000000 svgsimplegraph-0.2.1/svgsimplegraph.egg-info/requires.txt
--rw-r--r--   0 garrettpetersen   (501) staff       (20)       21 2024-03-27 22:54:27.000000 svgsimplegraph-0.2.1/svgsimplegraph.egg-info/top_level.txt
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-03-27 22:54:27.735631 svgsimplegraph-0.2.1/tests/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)        0 2023-05-30 04:47:02.000000 svgsimplegraph-0.2.1/tests/__init__.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     2778 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.1/tests/test_bubble_and_arrow.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     6853 2024-03-27 22:53:39.000000 svgsimplegraph-0.2.1/tests/test_categorical.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1700 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.1/tests/test_gist.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     3562 2024-02-11 22:35:12.000000 svgsimplegraph-0.2.1/tests/test_readme_examples.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1116 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.1/tests/test_ribbon.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-05 23:33:34.545918 svgsimplegraph-0.2.2/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1072 2023-05-30 04:47:02.000000 svgsimplegraph-0.2.2/LICENSE
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-05 23:33:34.545620 svgsimplegraph-0.2.2/PKG-INFO
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     6599 2024-02-12 21:11:46.000000 svgsimplegraph-0.2.2/README.md
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)       38 2024-04-05 23:33:34.546005 svgsimplegraph-0.2.2/setup.cfg
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      957 2024-04-05 23:32:24.000000 svgsimplegraph-0.2.2/setup.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-05 23:33:34.540940 svgsimplegraph-0.2.2/svgsimplegraph/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      124 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.2/svgsimplegraph/__init__.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    10527 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.2/svgsimplegraph/base.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    16487 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.2/svgsimplegraph/bubble_and_arrow.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    42467 2024-04-05 23:32:24.000000 svgsimplegraph-0.2.2/svgsimplegraph/categorical.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    15007 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.2/svgsimplegraph/ribbon.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    10208 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.2/svgsimplegraph/utils.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-05 23:33:34.542414 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-05 23:33:34.000000 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/PKG-INFO
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      524 2024-04-05 23:33:34.000000 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/SOURCES.txt
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)        1 2024-04-05 23:33:34.000000 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/dependency_links.txt
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)       17 2024-04-05 23:33:34.000000 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/requires.txt
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)       21 2024-04-05 23:33:34.000000 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/top_level.txt
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-05 23:33:34.544965 svgsimplegraph-0.2.2/tests/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)        0 2023-05-30 04:47:02.000000 svgsimplegraph-0.2.2/tests/__init__.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     2778 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.2/tests/test_bubble_and_arrow.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     7535 2024-04-05 23:32:24.000000 svgsimplegraph-0.2.2/tests/test_categorical.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1700 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.2/tests/test_gist.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     3562 2024-02-11 22:35:12.000000 svgsimplegraph-0.2.2/tests/test_readme_examples.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1116 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.2/tests/test_ribbon.py
```

### Comparing `svgsimplegraph-0.2.1/LICENSE` & `svgsimplegraph-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.1/PKG-INFO` & `svgsimplegraph-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgsimplegraph
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple SVG graphing package
 Author: Garrett M. Petersen
 Author-email: garrett.m.petersen@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/GarrettPetersen/svgsimplegraph
 Keywords: graph,svg,base64,svg simple graph
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `svgsimplegraph-0.2.1/README.md` & `svgsimplegraph-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.1/setup.py` & `svgsimplegraph-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Read in the README.md for the long description on PyPI
 with open("README.md", "r") as f:
     long_description = f.read()
 
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 DESCRIPTION = "Simple SVG graphing package"
 
 setup(
     name="svgsimplegraph",
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
```

### Comparing `svgsimplegraph-0.2.1/svgsimplegraph/base.py` & `svgsimplegraph-0.2.2/svgsimplegraph/base.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.1/svgsimplegraph/bubble_and_arrow.py` & `svgsimplegraph-0.2.2/svgsimplegraph/bubble_and_arrow.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.1/svgsimplegraph/categorical.py` & `svgsimplegraph-0.2.2/svgsimplegraph/categorical.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,40 @@
 
 def stacked_bar_range(data, series_types, secondary, maximum, minimum):
     non_secondary_bars_to_use = [
         not secondary[index] and series_types[index][0] == "bar"
         for index in range(len(secondary))
     ]
 
+    non_secondary_non_bars_to_use = [
+        not secondary[index] and series_types[index][0] != "bar"
+        for index in range(len(secondary))
+    ]
+
+    if any(non_secondary_non_bars_to_use):
+        non_secondary_non_bar_values = [
+            value
+            for values, non_bar_non_secondary in zip(
+                data, non_secondary_non_bars_to_use
+            )
+            if non_bar_non_secondary
+            for value in values
+            if value is not None  # Exclude None values
+        ]
+        max_non_secondary_non_bar = max(non_secondary_non_bar_values)
+        min_non_secondary_non_bar = min(non_secondary_non_bar_values)
+        if maximum is not None:
+            maximum = max(max_non_secondary_non_bar, maximum)
+        else:
+            maximum = max_non_secondary_non_bar
+        if minimum is not None:
+            minimum = min(min_non_secondary_non_bar, minimum)
+        else:
+            minimum = min_non_secondary_non_bar
+
     stacked_positive_data = [
         sum(
             max(value or 0, 0)
             for i, value in enumerate(column)
             if non_secondary_bars_to_use[i] and value is not None
         )
         for column in zip(*data)
```

### Comparing `svgsimplegraph-0.2.1/svgsimplegraph/ribbon.py` & `svgsimplegraph-0.2.2/svgsimplegraph/ribbon.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.1/svgsimplegraph/utils.py` & `svgsimplegraph-0.2.2/svgsimplegraph/utils.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.1/svgsimplegraph.egg-info/PKG-INFO` & `svgsimplegraph-0.2.2/svgsimplegraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgsimplegraph
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple SVG graphing package
 Author: Garrett M. Petersen
 Author-email: garrett.m.petersen@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/GarrettPetersen/svgsimplegraph
 Keywords: graph,svg,base64,svg simple graph
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `svgsimplegraph-0.2.1/svgsimplegraph.egg-info/SOURCES.txt` & `svgsimplegraph-0.2.2/svgsimplegraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.1/tests/test_bubble_and_arrow.py` & `svgsimplegraph-0.2.2/tests/test_bubble_and_arrow.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.1/tests/test_categorical.py` & `svgsimplegraph-0.2.2/tests/test_categorical.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,9 +212,31 @@
     graph.x_labels = [f"Label {i}" for i in range(number_of_bars)]
     graph.x_axis_label = "X Axis"
     graph.primary_y_axis_label = "Primary Y Axis"
     graph.secondary_y_axis_label = "Secondary Y Axis"
 
     graph.add_series([abs(i - number_of_bars // 2) for i in range(number_of_bars)])
 
+    large_base64 = graph.to_base64_src()
+    print(f"\n<img src='{large_base64}' />")
+
+    # New graph with stacked primary and line secondary
+    graph = CategoricalGraph(
+        width=600,
+        height=400,
+        bar_width=30,
+        title="Categorical Graph",
+        secondary_tick_suffix="%",
+        stacked=True,
+    )
+
+    graph.x_labels = [f"Label {i}" for i in range(5)]
+    graph.x_axis_label = "X Axis"
+    graph.primary_y_axis_label = "Primary Y Axis"
+    graph.secondary_y_axis_label = "Secondary Y Axis"
+
+    graph.add_series([1, 2, 3, 4, 5])
+    graph.add_series([50, 40, 30, 20, 10], series_type="line", secondary=True)
+    graph.add_series([3, 4, 3, 2, 1])
+
     stacked_base64 = graph.to_base64_src()
     print(f"\n<img src='{stacked_base64}' />")
```

### Comparing `svgsimplegraph-0.2.1/tests/test_gist.py` & `svgsimplegraph-0.2.2/tests/test_gist.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.1/tests/test_readme_examples.py` & `svgsimplegraph-0.2.2/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.1/tests/test_ribbon.py` & `svgsimplegraph-0.2.2/tests/test_ribbon.py`

 * *Files identical despite different names*

