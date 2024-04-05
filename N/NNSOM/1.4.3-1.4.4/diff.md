# Comparing `tmp/nnsom-1.4.3.tar.gz` & `tmp/nnsom-1.4.4.tar.gz`

## Comparing `nnsom-1.4.3.tar` & `nnsom-1.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    59032 2020-02-02 00:00:00.000000 nnsom-1.4.3/src/NNSOM/plots.py
--rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.4.3/src/NNSOM/som.py
--rw-r--r--   0        0        0    20699 2020-02-02 00:00:00.000000 nnsom-1.4.3/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.4.3/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.3/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.3/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0    58903 2020-02-02 00:00:00.000000 nnsom-1.4.4/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.4.4/src/NNSOM/som.py
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.4.4/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.4.4/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.4/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.4/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.4/PKG-INFO
```

### Comparing `nnsom-1.4.3/src/NNSOM/plots.py` & `nnsom-1.4.4/src/NNSOM/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .som import SOM
 from .utils import *
 
 import numpy as np
 import matplotlib.pyplot as plt
+from mpl_toolkits.axes_grid1 import make_axes_locatable
 import matplotlib.cm as cm
 from matplotlib.widgets import Button
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 import matplotlib.colors as mcolors
 class SOMPlots(SOM):
     """
     SOMPlots extends the SOM class by adding visualization capabilities to
@@ -294,62 +295,52 @@
             patches[neuron][0]._facecolor = color
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches, text
 
-    def color_hist(self, x, avg, mouse_click=False, **kwargs):
+
+
+    def color_hist(som, x, avg, mouse_click=False, connect_pick_event=True, **kwargs):
         # Plot an SOM figure where the size of the hexagons is related to
         # the number of elements in the clusters, and the color of the
         # inner hexagon is coded to the variable avg, which could be the
         # average number of a certain type of bond in the cluster
 
         # Find the maximum value of avg across all clusters
         dmax = np.amax(np.abs(avg))
-        numNeurons = self.numNeurons
+        numNeurons = som.numNeurons
 
-        fig, ax, patches, text = self.hit_hist(x, False, mouse_click, **kwargs)
+        fig, ax, patches, text = som.hit_hist(x, False, mouse_click, **kwargs)
 
         # Use the jet color map
         cmap = plt.get_cmap('jet')
         xx = np.zeros(numNeurons)
 
         # Adjust the color of the hexagon according to the avg value
         for neuron in range(numNeurons):
-            xx[neuron] = avg[neuron] / dmax
-            color = cmap(xx[neuron])
+            xx[neuron] = avg[neuron] / dmax  # Normalize avg values for mapping
+            color = cmap((xx[neuron] + 1) / 2)  # Adjust to cmap's scale (0 to 1)
             patches[neuron][0]._facecolor = color
 
-        plt.tight_layout()
+        # Correct way to use ScalarMappable for the colorbar
+        norm = plt.Normalize(vmin=-dmax, vmax=dmax)
+        sm = cm.ScalarMappable(cmap=cmap, norm=norm)
+        sm.set_array([])  # You can safely set it to an empty list.
+
+        # Add the colorbar to the figure
+        divider = make_axes_locatable(ax)
+        cax = divider.append_axes("right", size="5%", pad=0.05)
+        cbar = fig.colorbar(sm, cax=cax)
 
-        # # Add a color bar the the figure to indicate levels
-        # # create an axes on the right side of ax. The width of cax will be 5%
-        # # of ax and the padding between cax and ax will be fixed at 0.05 inch.
-        # divider = make_axes_locatable(ax)
-        # cax = divider.append_axes("right", size="5%", pad=0.05)
-        #
-        # cbar = plt.colorbar(ax, cax=cax, cmap=cmap)
-
-        cax = cm.ScalarMappable(cmap=cmap)
-        cax.set_array(xx)
-        cbar = fig.colorbar(ax=ax, cax=cax)
-
-        # Adjust the tick labels to the correct scale
-        ticklab = cbar.ax.get_yticks()
-        numticks = len(ticklab)
-        ticktext = []
-        for i in range(numticks):
-            ticktext.append('%.2f' % (dmax * ticklab[i]))
-
-        cbar.ax.set_yticklabels(ticktext)
-
-        # Get rid of extra white space on sides
-        fig.tight_layout()
+        # Adjust the tick labels if necessary (e.g., to represent avg values)
+        # This part might need adjustment based on your specific requirements.
 
+        plt.tight_layout()
         return fig, patches, text, cbar
 
     def cmplx_hit_hist(self, x, clust, perc, ind_missClass, ind21, ind12, mouse_click=False, **kwargs):
         """ Generates a complex hit histogram.
         It indicates what the majority class in each cluster is, and how many specific class occur in each cluster.
 
         Args:
```

### Comparing `nnsom-1.4.3/src/NNSOM/som.py` & `nnsom-1.4.4/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.4.3/src/NNSOM/utils.py` & `nnsom-1.4.4/src/NNSOM/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,39 @@
             cluster_array[i] = feature[cluster_indices]
         else:
             cluster_array[i] = np.array([])  # Store an empty array if the cluster is empty
 
     return cluster_array
 
 
+def get_cluster_avg(feature, clust):
+    """
+    Returns the average value of a feature for each cluster.
+
+    Parameters
+    ----------
+    feature : array-like
+        Feature array.
+    clust : list
+        A list of cluster arrays, each containing indices sorted by distances.
+
+    Returns
+    -------
+    cluster_avg : numpy array
+        A cluster array with the average value of the feature for each cluster.
+    """
+    cluster_array = get_cluster_array(feature, clust)
+    cluster_avg = np.zeros(len(cluster_array))
+    for i in range(len(cluster_array)):
+        if len(cluster_array[i]) > 0:
+            cluster_avg[i] = np.mean(cluster_array[i])
+
+    return cluster_avg
+
+
 def closest_class_cluster(cat_feature, clust):
     """
     Returns the cluster array with the closest class for each cluster.
 
     Paramters
     ----------
     cat_feature : array-like
@@ -572,15 +597,15 @@
         A tuple (min_value, max_value) where min_value is the minimum value
         in the data, and max_value is the maximum value.
     """
     flat_list = flatten(data)
     return min(flat_list), max(flat_list)
 
 
-def get_edge_width(indices, clust):
+def get_edge_widths(indices, clust):
     """ Calculate edge width for each cluster based on the number of indices in the cluster.
 
     Args:
         indices: 1-d array
             Array of indices for the specific class.
         clust: sequence of vectors
             A sequence of vectors, each containing the indices of elements in a cluster.
@@ -600,42 +625,66 @@
                 lwidth[i] = None
         else:
             lwidth[i] = None
 
     return lwidth
 
 
-def get_edge_color(clust, *args):
-    """ Calculate edge color for each cluster based on the number of indices in the cluster.
+def get_color_labels(clust, *listOfIndices):
+    """ Generates color label for each cluster based on indices of classes.
 
     Args:
         clust: sequence of vectors
             A sequence of vectors, each containing the indices of elements in a cluster.
 
         *args: 1-d array
             A list of indices where the specific class is present.
     """
+    # Validate if the user have provided at least one class indices
+    if len(listOfIndices) == 0:
+        raise ValueError('At least one class indices must be provided.')
+
+    # Validate if the arg is a list or numpy array and unpack them
+    numst = []
+    for arg in listOfIndices:
+        if not isinstance(arg, (list, np.ndarray)):
+            raise ValueError('The arguments must be a list or numpy array.')
+        else:
+            numst.append(arg)
 
-    # unpack the args
-    numst = list(args)
+            # Initialize the color label array
+    color_labels = np.zeros(len(clust))
 
-    # Initialize the edge color array
-    edge_color = np.zeros(len(clust))
+    # When there is only one list provides,
+    # check if the cluster contains the indices of the class.
+    # If that class is majority in the cluster, assign 1, otherwise 0.
+    if len(numst) == 1:
+        indices = numst[0]
+        for i in range(len(clust)):
+            if len(clust[i]) != 0:
+                num_class = len(np.intersect1d(clust[i], indices))
+                if num_class > len(clust[i]) / 2:
+                    color_labels[i] = 1
+                else:
+                    color_labels[i] = 0
+            else:
+                color_labels[i] = None
 
-    # Detect the intersection of the cluster and each list of indices (class),
-    # and get the majority class in the cluster.
-    # Append the majority class to the edge color array.
-    for i in range(len(clust)):
-        if len(clust[i]) != 0:
-            intersection = [len(np.intersect1d(clust[i], numst[j])) for j in range(len(numst))]
-            edge_color[i] = np.argmax(intersection)
-        else:
-            edge_color[i] = None
+    else:
+        # Detect the intersection of the cluster and each list of indices (class),
+        # and get the majority class in the cluster.
+        # Append the majority class to the edge color array.
+        for i in range(len(clust)):
+            if len(clust[i]) != 0:
+                intersection = [len(np.intersect1d(clust[i], numst[j])) for j in range(len(numst))]
+                color_labels[i] = np.argmax(intersection)
+            else:
+                color_labels[i] = None
 
-    return edge_color
+    return color_labels
 
 
 # Helper functions to create button objects in the interactive plot
 def create_buttons(fig, button_types):
     sidebar_width = 0.2
     button_config = calculate_button_positions(len(button_types), sidebar_width)
```

### Comparing `nnsom-1.4.3/.gitignore` & `nnsom-1.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.4.3/pyproject.toml` & `nnsom-1.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.4.3"
+version = "1.4.4"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.4.3/PKG-INFO` & `nnsom-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.4.3
+Version: 1.4.4
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

