# Comparing `tmp/nnsom-1.4.4.tar.gz` & `tmp/nnsom-1.4.5.tar.gz`

## Comparing `nnsom-1.4.4.tar` & `nnsom-1.4.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    58903 2020-02-02 00:00:00.000000 nnsom-1.4.4/src/NNSOM/plots.py
--rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.4.4/src/NNSOM/som.py
--rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.4.4/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.4.4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.4/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.4/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0    58907 2020-02-02 00:00:00.000000 nnsom-1.4.5/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.4.5/src/NNSOM/som.py
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.4.5/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.4.5/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.5/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.5/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.5/PKG-INFO
```

### Comparing `nnsom-1.4.4/src/NNSOM/plots.py` & `nnsom-1.4.5/src/NNSOM/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,25 +297,25 @@
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches, text
 
 
 
-    def color_hist(som, x, avg, mouse_click=False, connect_pick_event=True, **kwargs):
+    def color_hist(self , x, avg, mouse_click=False, connect_pick_event=True, **kwargs):
         # Plot an SOM figure where the size of the hexagons is related to
         # the number of elements in the clusters, and the color of the
         # inner hexagon is coded to the variable avg, which could be the
         # average number of a certain type of bond in the cluster
 
         # Find the maximum value of avg across all clusters
         dmax = np.amax(np.abs(avg))
-        numNeurons = som.numNeurons
+        numNeurons = self.numNeurons
 
-        fig, ax, patches, text = som.hit_hist(x, False, mouse_click, **kwargs)
+        fig, ax, patches, text = self.hit_hist(x, False, mouse_click, **kwargs)
 
         # Use the jet color map
         cmap = plt.get_cmap('jet')
         xx = np.zeros(numNeurons)
 
         # Adjust the color of the hexagon according to the avg value
         for neuron in range(numNeurons):
```

### Comparing `nnsom-1.4.4/src/NNSOM/som.py` & `nnsom-1.4.5/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.4.4/src/NNSOM/utils.py` & `nnsom-1.4.5/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.4.4/.gitignore` & `nnsom-1.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.4.4/pyproject.toml` & `nnsom-1.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.4.4"
+version = "1.4.5"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.4.4/PKG-INFO` & `nnsom-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.4.4
+Version: 1.4.5
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

