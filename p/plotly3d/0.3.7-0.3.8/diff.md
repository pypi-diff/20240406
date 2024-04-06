# Comparing `tmp/plotly3d-0.3.7.tar.gz` & `tmp/plotly3d-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.3.7.tar", last modified: Fri Apr  5 06:14:45 2024, max compression
+gzip compressed data, was "plotly3d-0.3.8.tar", last modified: Sat Apr  6 19:12:16 2024, max compression
```

## Comparing `plotly3d-0.3.7.tar` & `plotly3d-0.3.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:14:45.782286 plotly3d-0.3.7/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.3.7/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-05 06:14:45.781469 plotly3d-0.3.7/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.3.7/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:14:45.776069 plotly3d-0.3.7/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.3.7/plotly3d/__init__.py
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9559 2024-04-05 06:14:14.000000 plotly3d-0.3.7/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:14:45.780373 plotly3d-0.3.7/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-05 06:14:45.776977 plotly3d-0.3.7/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-05 06:14:45.778079 plotly3d-0.3.7/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-05 06:14:45.779252 plotly3d-0.3.7/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-05 06:14:45.780023 plotly3d-0.3.7/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-05 06:14:45.780721 plotly3d-0.3.7/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-05 06:14:45.782567 plotly3d-0.3.7/setup.cfg
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-05 06:14:40.000000 plotly3d-0.3.7/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-06 19:12:16.861240 plotly3d-0.3.8/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.3.8/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-06 19:12:16.860337 plotly3d-0.3.8/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.3.8/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-06 19:12:16.855703 plotly3d-0.3.8/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.3.8/plotly3d/__init__.py
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9576 2024-04-06 19:11:13.000000 plotly3d-0.3.8/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-06 19:12:16.859675 plotly3d-0.3.8/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-06 19:12:16.856371 plotly3d-0.3.8/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-06 19:12:16.857162 plotly3d-0.3.8/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-06 19:12:16.858547 plotly3d-0.3.8/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-06 19:12:16.859152 plotly3d-0.3.8/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-06 19:12:16.859742 plotly3d-0.3.8/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-06 19:12:16.866969 plotly3d-0.3.8/setup.cfg
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-06 19:11:40.000000 plotly3d-0.3.8/setup.py
```

### Comparing `plotly3d-0.3.7/LICENSE` & `plotly3d-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly3d-0.3.7/plotly3d/plot.py` & `plotly3d-0.3.8/plotly3d/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,117 +1,119 @@
 import plotly.graph_objects as go
 from sklearn.preprocessing import MinMaxScaler
 import numpy as np
 import pandas as pd
-import os
+import matplotlib.pyplot as plt
+import matplotlib
 
 def scatter(points, colors=None, **kwargs):
     """
     Plots 3D scatter plot with optional rescaling, coloring, and customization.
     
     Parameters:
     - points: Array of points to plot.
     - colors: Optional array of colors for each point.
     - scaler: Optional scaler object to rescale points. If None and rescaling is enabled, MinMaxScaler is used.
     - **kwargs: Additional optional arguments:
         - s (float): Size of the markers.
         - alpha (float): Opacity of the markers.
-        - force_continuous (bool): Force treating colors as continuous even if they seem categorical.
+        - force_continuous (bool): When True, applies a continuous colormap but discretizes it for categorical data.
         - title (str): Title of the plot.
         - filename (str): If provided, saves the plot to this file.
         - rescale (bool): If True, rescales points using the provided or default scaler.
         - fig (go.Figure): Plotly figure object to which the scatter plot will be added. If None, a new figure is created.
         - xtitle (str), ytitle (str), ztitle (str): Titles for the X, Y, and Z axes.
+        - colorscale (str): Colormap to use ('Viridis', 'Inferno', etc.).
+        - legend (bool): Whether to show legend.
     """
     is_3d = points.shape[1] == 3
     plot_func = go.Scatter3d if is_3d else go.Scatter
     scaler = kwargs.get('scaler', None)
-    s = kwargs.get('s', 1)
-    alpha = kwargs.get('alpha', 1)
+    s = kwargs.get('s', 6)  # Default size
+    alpha = kwargs.get('alpha', 0.8)  # Default opacity
     title = kwargs.get('title', 'Plot')
     filename = kwargs.get('filename', None)
     xtitle = kwargs.get('xtitle', 'X')
     ytitle = kwargs.get('ytitle', 'Y')
     ztitle = kwargs.get('ztitle', 'Z')
     force_continuous = kwargs.get('force_continuous', False)
     rescale = kwargs.get('rescale', True)
     legend = kwargs.get('legend', True)
-    colorscale = kwargs.get('colorscale', 'Viridis')
+    colorscale = kwargs.get('colorscale', 'Viridis').capitalize()  # Ensure correct case
     fig = kwargs.get('fig', go.Figure())
     points = np.asarray(points)
     colors = np.asarray(colors) if colors is not None else None
+    
     if rescale:
         if scaler is None:
             scaler = MinMaxScaler()
             scaler.fit(points)
         points_s = scaler.transform(points)
     else:
         points_s = points
 
     if colors is None:
         colors = np.zeros(points.shape[0])
         is_categorical = True
     else:
-        # Step 1: Determine Color Type
         unique_colors = np.unique(colors)
-        is_categorical = (len(unique_colors) / len(colors) < 0.05) and not force_continuous # Heuristic threshold
-        # Step 2: Preprocess Points
-    if is_categorical:
-        # Step 3: Categorical Colors Plotting Strategy
-        # Map categorical color labels to integers
-        color_map, categories = pd.factorize(colors, sort=True)
-        # Create a trace for each unique color/category
-        for i, color in enumerate(categories):
-            idx = color_map == i
-            if is_3d:
-                fig.add_trace(plot_func(
-                    x=points_s[idx, 0],
-                    y=points_s[idx, 1],
-                    z=points_s[idx, 2],
-                    mode='markers',
-                    marker=dict(size=s, opacity=alpha, color=i), # Use integer mapping for color
-                    name=str(color)  # Use actual category name for legend
-                ))
-            else:
-                fig.add_trace(plot_func(
-                    x=points_s[idx, 0],
-                    y=points_s[idx, 1],
-                    mode='markers',
-                    marker=dict(size=s, opacity=alpha, color=i), # Use integer mapping for color
-                    name=str(color)  # Use actual category name for legend
-                ))
+        is_categorical = not force_continuous and (len(unique_colors) / len(colors) < 0.05)
+    
+    if force_continuous and colors is not None and is_categorical:
+        # Normalize color values for continuous colormap application
+        color_map, _ = pd.factorize(colors, sort=True)
+        color_vals = MinMaxScaler().fit_transform(color_map.reshape(-1, 1)).flatten()
+        cmap = plt.get_cmap(colorscale)
+        discrete_mapping = cmap(color_vals)  # Apply colormap
+        
+        hex_colors = [matplotlib.colors.rgb2hex(color) for color in discrete_mapping]  # Convert to hex
+
+        fig.add_trace(plot_func(
+            x=points_s[:, 0],
+            y=points_s[:, 1],
+            z=points_s[:, 2] if is_3d else None,
+            mode='markers',
+            marker=dict(size=s, color=hex_colors, opacity=alpha),
+            hoverinfo='text',
+            text=colors,  # Show original category names on hover
+        ))
     else:
-        # Step 3: Continuous Colors Plotting Strategy
+        # Continuous or non-force_continuous categorical handling
         if is_3d:
             fig.add_trace(plot_func(
                 x=points_s[:, 0],
                 y=points_s[:, 1],
                 z=points_s[:, 2],
                 mode='markers',
-                marker=dict(size=s, color=colors, colorscale='Viridis', opacity=alpha, colorbar=dict(title='Color Scale')),
+                marker=dict(size=s, color=colors, colorscale=colorscale, opacity=alpha, colorbar=dict(title='Color Scale') if not is_categorical else None),
             ))
         else:
             fig.add_trace(plot_func(
                 x=points_s[:, 0],
                 y=points_s[:, 1],
                 mode='markers',
-                marker=dict(size=s, color=colors, colorscale='Viridis', opacity=alpha, colorbar=dict(title='Color Scale')),
+                marker=dict(size=s, color=colors, colorscale=colorscale, opacity=alpha, colorbar=dict(title='Color Scale') if not is_categorical else None),
             ))
-    
-    fig.data[0].marker.colorscale = colorscale
+
+    # Layout updates
     if is_3d:
         fig.update_layout(
             title=title,
-            scene=dict(xaxis_title=xtitle, yaxis_title=ytitle, zaxis_title=ztitle),
+            scene=dict(
+                xaxis_title=xtitle,
+                yaxis_title=ytitle,
+                zaxis_title=ztitle
+            ),
             showlegend=legend
         )
     else:
         fig.update_layout(
             title=title,
-            xaxis_title=xtitle, yaxis_title=ytitle,
+            xaxis_title=xtitle,
+            yaxis_title=ytitle,
             showlegend=legend
         )
     if filename is not None:
         fig.write_html(filename)
 
     return fig
```

