# Comparing `tmp/PyComplexHeatmap-1.6.9.tar.gz` & `tmp/PyComplexHeatmap-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.6.9.tar", last modified: Fri Apr  5 03:51:44 2024, max compression
+gzip compressed data, was "PyComplexHeatmap-1.7.0.tar", last modified: Sat Apr  6 18:33:36 2024, max compression
```

## Comparing `PyComplexHeatmap-1.6.9.tar` & `PyComplexHeatmap-1.7.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.211295 PyComplexHeatmap-1.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.179295 PyComplexHeatmap-1.6.9/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.179295 PyComplexHeatmap-1.6.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.183295 PyComplexHeatmap-1.6.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-05 03:51:44.211295 PyComplexHeatmap-1.6.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.183295 PyComplexHeatmap-1.6.9/PyComplexHeatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 03:51:43.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    63027 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    79542 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    20240 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.211295 PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-05 03:51:43.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-05 03:51:44.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:51:43.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 03:51:43.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.211295 PyComplexHeatmap-1.6.9/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/ComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/ComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/PyComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/PyComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/README.md
--rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/beta.csv
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/compare.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/df_col.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/df_row.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/heatmap.R
--rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-05 03:51:23.000000 PyComplexHeatmap-1.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:51:44.211295 PyComplexHeatmap-1.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 03:51:23.000000 PyComplexHeatmap-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.068538 PyComplexHeatmap-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.036538 PyComplexHeatmap-1.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.036538 PyComplexHeatmap-1.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.036538 PyComplexHeatmap-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-06 18:33:36.068538 PyComplexHeatmap-1.7.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.040538 PyComplexHeatmap-1.7.0/PyComplexHeatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 18:33:34.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63135 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79542 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21771 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.068538 PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-06 18:33:35.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-06 18:33:36.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:33:35.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 18:33:35.000000 PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:36.068538 PyComplexHeatmap-1.7.0/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/ComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/ComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/PyComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/PyComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/README.md
+-rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/beta.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/compare.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/df_col.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/df_row.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/heatmap.R
+-rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-06 18:33:11.000000 PyComplexHeatmap-1.7.0/comparison/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-06 18:33:12.000000 PyComplexHeatmap-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:33:36.068538 PyComplexHeatmap-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-06 18:33:12.000000 PyComplexHeatmap-1.7.0/setup.py
```

### Comparing `PyComplexHeatmap-1.6.9/.github/FUNDING.yml` & `PyComplexHeatmap-1.7.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/.github/ISSUE_TEMPLATE/bug_report.md` & `PyComplexHeatmap-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/.github/ISSUE_TEMPLATE/feature_request.md` & `PyComplexHeatmap-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/.github/workflows/python-publish.yml` & `PyComplexHeatmap-1.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/CITATION.cff` & `PyComplexHeatmap-1.7.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/LICENSE` & `PyComplexHeatmap-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/PKG-INFO` & `PyComplexHeatmap-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.6.9
+Version: 1.7.0
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
```

### Comparing `PyComplexHeatmap-1.6.9/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.7.0/PyComplexHeatmap/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,15 +522,18 @@
 			relpos=rp,
 			patchA=None,
 			patchB=None,
 			connectionstyle=None,
 		)
 		# arrow: ->, from text to point.
 		# self.plot_kws.setdefault('transform_rotates_text', False)
-		self.plot_kws.setdefault("arrowprops", arrowprops)
+		self.plot_kws.setdefault("arrowprops", {})
+		for k in arrowprops:
+			if k not in self.plot_kws['arrowprops']:
+				self.plot_kws['arrowprops'][k]=arrowprops[k]
 		self.plot_kws.setdefault("rotation_mode", "anchor")
 
 	def _calculate_colors(self):  # add self.color_dict (each col is a dict)
 		self.color_dict = {}
 		col = self.df.columns.tolist()[0]
 		if get_colormap(self.cmap).N < 256 or self.df.dtypes[col] == object:
 			cc_list = (
```

### Comparing `PyComplexHeatmap-1.6.9/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.7.0/PyComplexHeatmap/clustermap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.7.0/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.7.0/PyComplexHeatmap/dotHeatmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	data,
 	hue=None,
 	vmin=None,
 	vmax=None,
 	ax=None,
 	colors=None,
 	cmap=None,
-	ratio=None,
+	max_s=None,
 	spines=False,
 	**kwargs
 ):
 	"""
 	Plot dot heatmap using a dataframe matrix as input.
 
 	Parameters
@@ -81,33 +81,39 @@
 	if ax is None:
 		ax = plt.gca()
 	df = data["Col"].apply(lambda j: col_labels.index(j) + 1).to_frame(name="X")
 	df["Y"] = data["Row"].apply(lambda j: row_labels.index(j) + 1)
 	df["Value"] = data.Value.values
 	del data
 
-	if ratio is None:
+	if max_s is None: #passed from DotClustermapPlotter, not None
+		#The unit of size for the s parameter is squared points. This means
+		# that the area of the marker is specified in points squared.
+		# A point in this context is a unit of measure in typography,
+		# equal to 1/72 of an inch. Therefore, if you specify s=100,
+		# each marker's area will be 100 points squared, not its width or height.
 		w, h = (
 			ax.get_window_extent().width / ax.figure.dpi,
 			ax.get_window_extent().height / ax.figure.dpi,
-		)
+		) #unit is inch
 		r = min(w * 72 / len(col_labels), h * 72 / len(row_labels))
-		ratio = r**2
-
+		# r is the minimal of width and height for each scatter point, unit is point.
+		max_s = r**2
 	# s
 	s = kwargs.pop("s", None)
+	# print(s is None,vmin,vmax)
 	if s is None:
 		df["S"] = scale(df["Value"].abs().values,vmin=vmin, vmax=vmax)
 	else:
 		if isinstance(s, pd.DataFrame):
 			s = s.reindex(index=row_labels, columns=col_labels).stack().reset_index()
 			s.columns = ["Row", "Col", "Value"]
 			# print(s.shape)
 			# print(s.head())
-			df["S"] = scale(s.Value.abs().values,vmin=vmin, vmax=vmax)
+			df["S"] = scale(s.Value.abs().values) #scale to 0-1
 			# df['S'] = s.Value.values
 		elif isinstance(s, (int, float)):
 			df["S"] = s
 
 	# hue
 	if not hue is None:  # hue is a dataframe
 		hue = hue.reindex(index=row_labels, columns=col_labels).stack().reset_index()
@@ -166,26 +172,28 @@
 			raise ValueError("colors must be string or dict")
 
 		df["C"] = df["Hue"].map(color_dict)
 		c_ready = True
 	kwargs.setdefault(
 		"norm", matplotlib.colors.Normalize(vmin=vmin, vmax=vmax, clip=True)
 	)
+
+	# print(f"max_s: {max_s}",df.S.min(),df.S.max()) #min and max S should be 0,1
 	if c_ready and type(cmap) == str:
 		kwargs["cmap"] = cmap
 		for mk in df.Markers.unique():
 			# df1 = df.query("Markers==@mk").copy()
 			df1 = df.loc[df.Markers==mk].copy()
 			if df1.shape[0] == 0:
 				continue
 			kwargs["marker"] = mk
 			ax.scatter(
 				x=df1.X.values,
 				y=df1.Y.values,
-				s=df1.S * ratio,
+				s=df1.S * max_s,
 				c=df1.C.values,
 				**kwargs
 			)  # vmax=vmax,vmin=vmin,
 	elif type(cmap) == dict and not hue is None:
 		for h in cmap:  # key are hue, values are cmap
 			# df1 = df.query("Hue==@h").copy()
 			df1 = df.loc[df.Hue==h].copy()
@@ -204,15 +212,15 @@
 			for mk in df1.Markers.unique():
 				# df2 = df1.query("Markers==@mk").copy()
 				df2 = df1.loc[df1.Markers==mk].copy()
 				kwargs["marker"] = mk
 				ax.scatter(
 					x=df2.X.values,
 					y=df2.Y.values,
-					s=df2.S * ratio,
+					s=df2.S * max_s,
 					c=df2.C.values,
 					**kwargs
 				)  #
 	else:
 		raise ValueError("cmap must be string or dict")
 
 	ax.set_ylim([0.5, len(row_labels) + 0.5])
@@ -261,16 +269,14 @@
 	marker :str or dict, optional.
 		Please go to: https://matplotlib.org/stable/api/markers_api.html to see all available markers.
 		Such as '.',',','o','v','^','<','>','1','2','3','4','8','s','p','P','*','h','H','+','x','X','D','d','|','_',
 		default marker is 'o'.
 		If marker is a string, it should be a marker to control the markers of scatter (dot).
 		marker could also be a name of the column from data.columns.tolist()
 		If marker is a dict, the keys should be the values from data[hue].values, and values should be marker.
-	alpha: float [0,1]
-		coefficient to scale the size of dot in figure legend, valid for marker and dot in legend.
 	colors :dict.
 		Keys should be the values from data[hue].values, and values should be color.
 		It will be only used to control the colors of markers in figure legend.
 	cmap :str or dict, optional.
 		If cmap is a dict, the keys should be the values from data[hue].values, and values should be cmap.
 		If cmap is a string, it should be colormap, such as 'Set1'.
 	color_legend_kws: dict
@@ -290,18 +296,20 @@
 	c_na : float, int or str
 		used to fill na for data.pivot_table(index=self.y,columns=self.x,values=self.c,aggfunc=self.aggfunc).fillna(self.c_na)
 	aggfunc : function
 		when there are multiple values for the same x and y, using aggfunc (default is np.mean) to aggregate them.
 		aggfunc will be called in data.pivot(index=y,columns=x,values=value,aggfunc=aggfunc)
 	spines: bool
 		Whether show spines of the axes or not [False]
-	ratio: float
-		the size of dot will be multipled by ratio.
+	max_s: float
+		max size of the dot in scatter, default is None, will be inferred automatically.
+	alpha: float [0,1]
+		coefficient to scale the size of dot in figure legend, valid for marker and dot in legend.
 	kwargs :dict
-		Other kwargs passed to ClusterMapPlotter and dotHeatmap2d, such as ratio, vmin, vmax.
+		Other kwargs passed to ClusterMapPlotter and dotHeatmap2d, such as max_s, vmin, vmax.
 
 	Returns
 	-------
 	DotClustermapPlotter.
 	"""
 	def __init__(
 		self,
@@ -313,21 +321,22 @@
 		s=None,
 		c=None,
 		marker="o",
 		alpha=1,
 		color_legend_kws={},
 		cmap_legend_kws={},
 		dot_legend_kws={},
+		dot_legend_marker="o",
 		aggfunc=np.mean,
 		value_na=0,
 		hue_na="NA",
 		s_na=0,
 		c_na=0,
 		spines=False,
-		ratio=None,
+		max_s=None,
 		**kwargs
 	):
 		kwargs["data"] = data
 		self.x = x
 		self.y = y
 		self.value = value
 		self.hue = hue
@@ -340,15 +349,16 @@
 		self.hue_na = hue_na
 		self.s_na = s_na
 		self.c_na = c_na
 		self.color_legend_kws = color_legend_kws
 		self.cmap_legend_kws = cmap_legend_kws
 		self.spines = spines
 		self.dot_legend_kws = dot_legend_kws
-		self.ratio=ratio
+		self.dot_legend_marker=dot_legend_marker
+		self.max_s=max_s
 
 		super().__init__(**kwargs)
 
 	def format_data(self, data, mask=None, z_score=None, standard_scale=None):
 		# self.data=data
 		data2d = data.pivot_table(
 			index=self.y, columns=self.x, values=self.value, aggfunc=self.aggfunc
@@ -432,24 +442,40 @@
 
 	def plot_matrix(self, row_order, col_order):
 		if self.verbose >= 1:
 			print("Plotting matrix..")
 		nrows = len(row_order)
 		ncols = len(col_order)
 
-		if self.ratio is None:
+		ratio=self.kwargs.pop('ratio',None)
+		if not ratio is None:
+			print("Warning: ratio is deprecated, please use max_s instead")
+		if self.max_s is None:
+			self.max_s = ratio
+
+		if self.max_s is None:
+			# The unit of size for the s parameter is squared points. This means
+			# that the area of the marker is specified in points squared.
+			# A point in this context is a unit of measure in typography,
+			# equal to 1/72 of an inch. Therefore, if you specify s=100,
+			# each marker's area will be 100 points squared, not its width or height.
 			w, h = (
 				self.ax_heatmap.get_window_extent().width / self.ax_heatmap.figure.dpi,
 				self.ax_heatmap.get_window_extent().height / self.ax_heatmap.figure.dpi,
-			)
+			) # unit is inch
 			r = min(w * 72 / self.data2d.shape[1], h * 72 / self.data2d.shape[0])
-			ratio = r ** 2
+			# r is the minimal of width and height for each scatter point, unit is point.
+			max_s = r ** 2
+			if self.verbose >= 1:
+				print(f"Inferred max_s (max size of scatter point) is: {max_s}")
 		else:
-			ratio = self.ratio
-		self.kwargs['ratio'] = ratio
+			max_s = self.max_s
+			if self.verbose >= 1:
+				print(f"Using user provided max_s: {max_s}")
+		self.kwargs['max_s'] = max_s
 		self.col_split_gap_pixel = self.col_split_gap * mm2inch * self.ax.figure.dpi
 		self.wspace = (
 			(self.col_split_gap_pixel * ncols)
 			/ (
 				self.ax_heatmap.get_window_extent().width
 				+ self.col_split_gap_pixel - self.col_split_gap_pixel * ncols
 			)
@@ -564,36 +590,36 @@
 			marker = self.kwargs.get("marker", None)
 			# ax = self.heatmap_axes[0, 0]
 			# w, h = (
 			#     ax.get_window_extent().width / ax.figure.dpi,
 			#     ax.get_window_extent().height / ax.figure.dpi,
 			# )
 			# r = min(w * 72 / len(self.col_order[0]), h * 72 / len(self.row_order[0]))
-			ratio=self.kwargs['ratio']
+			max_s=self.kwargs['max_s']
 			if type(marker) == dict and not self.hue is None:
 				self.legend_list.append(
 					[
-						(marker, self.kwargs.get("colors", None), np.sqrt(ratio) * self.alpha),
+						(marker, self.kwargs.get("colors", None), np.sqrt(max_s) * self.alpha),
 						self.hue,
 						self.dot_legend_kws,
 						len(marker),
 						"markers",
-					]
+					] #size of s in scatter equal to marker_size**2
 				)  # markersize is r*0.8
 			# dot size legend:
 			if type(self.s) == str:
 				# s=self.kwargs.get('s',None)
 				# colors=self.kwargs.get('colors',None)
 				markers1 = {}
 				ms = {}
 				for f in [1, 0.8, 0.6, 0.4, 0.2]:
 					k = str(round(f * self.smax, 2))
-					markers1[k] = "o"
-					ms[k] = f  * np.sqrt(ratio) * self.alpha
-					# ms[k] = np.sqrt(f * ratio * self.alpha)
+					markers1[k] = self.dot_legend_marker
+					ms[k] = f  * np.sqrt(max_s) * self.alpha
+					# ms[k] = np.sqrt(f * max_s * self.alpha)
 				title = self.s if not self.s is None else self.value
 				self.legend_list.append(
 					[
 						(markers1, None, ms),
 						title,
 						self.dot_legend_kws,
 						len(markers1),
```

### Comparing `PyComplexHeatmap-1.6.9/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.7.0/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.7.0/PyComplexHeatmap/oncoPrint.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.7.0/PyComplexHeatmap/utils.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.6.9
+Version: 1.7.0
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
```

### Comparing `PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/SOURCES.txt` & `PyComplexHeatmap-1.7.0/PyComplexHeatmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/README.md` & `PyComplexHeatmap-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/ComplexHeatmap.pdf` & `PyComplexHeatmap-1.7.0/comparison/ComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/ComplexHeatmap.png` & `PyComplexHeatmap-1.7.0/comparison/ComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/PyComplexHeatmap.pdf` & `PyComplexHeatmap-1.7.0/comparison/PyComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/PyComplexHeatmap.png` & `PyComplexHeatmap-1.7.0/comparison/PyComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/README.md` & `PyComplexHeatmap-1.7.0/comparison/README.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/beta.csv` & `PyComplexHeatmap-1.7.0/comparison/beta.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/df_col.csv` & `PyComplexHeatmap-1.7.0/comparison/df_col.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/df_row.csv` & `PyComplexHeatmap-1.7.0/comparison/df_row.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/heatmap.R` & `PyComplexHeatmap-1.7.0/comparison/heatmap.R`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/heatmap.ipynb` & `PyComplexHeatmap-1.7.0/comparison/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/comparison/heatmap.py` & `PyComplexHeatmap-1.7.0/comparison/heatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/pyproject.toml` & `PyComplexHeatmap-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.9/setup.py` & `PyComplexHeatmap-1.7.0/setup.py`

 * *Files identical despite different names*

