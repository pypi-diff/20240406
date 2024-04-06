# Comparing `tmp/geoglows-1.0.0rc2.tar.gz` & `tmp/geoglows-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.0.0rc2.tar", last modified: Sat Apr  6 17:39:10 2024, max compression
+gzip compressed data, was "geoglows-1.0.0rc3.tar", last modified: Sat Apr  6 18:46:02 2024, max compression
```

## Comparing `geoglows-1.0.0rc2.tar` & `geoglows-1.0.0rc3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.752873 geoglows-1.0.0rc2/
--rw-r--r--   0 rchales    (502) staff       (20)       98 2024-04-02 00:15:15.000000 geoglows-1.0.0rc2/.gitignore
--rw-r--r--   0 rchales    (502) staff       (20)      568 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/.readthedocs.yml
--rw-r--r--   0 rchales    (502) staff       (20)     1519 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/LICENSE
--rw-r--r--   0 rchales    (502) staff       (20)      173 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/MANIFEST.in
--rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 17:39:10.752566 geoglows-1.0.0rc2/PKG-INFO
--rw-r--r--   0 rchales    (502) staff       (20)      780 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/README.md
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.743621 geoglows-1.0.0rc2/docs/
--rw-r--r--   0 rchales    (502) staff       (20)      634 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/Makefile
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.743732 geoglows-1.0.0rc2/docs/_static/
--rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/_static/.gitkeep
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.743828 geoglows-1.0.0rc2/docs/_templates/
--rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/_templates/.gitkeep
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.744400 geoglows-1.0.0rc2/docs/api-documentation/
--rw-r--r--   0 rchales    (502) staff       (20)      321 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation/analysis.rst
--rw-r--r--   0 rchales    (502) staff       (20)      210 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation/bias.rst
--rw-r--r--   0 rchales    (502) staff       (20)      153 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation/examples.rst
--rw-r--r--   0 rchales    (502) staff       (20)      687 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation/plots.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1241 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation/streamflow.rst
--rw-r--r--   0 rchales    (502) staff       (20)      791 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1905 2024-03-29 16:40:36.000000 geoglows-1.0.0rc2/docs/conf.py
--rw-r--r--   0 rchales    (502) staff       (20)      871 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/dev-notes.rst
--rw-r--r--   0 rchales    (502) staff       (20)     2028 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/index.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1536 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/license.rst
--rw-r--r--   0 rchales    (502) staff       (20)      100 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/requirements.txt
--rw-r--r--   0 rchales    (502) staff       (20)      243 2024-04-02 00:15:15.000000 geoglows-1.0.0rc2/environment.yaml
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.745352 geoglows-1.0.0rc2/geoglows/
--rw-r--r--   0 rchales    (502) staff       (20)      418 2024-04-06 17:38:45.000000 geoglows-1.0.0rc2/geoglows/__init__.py
--rw-r--r--   0 rchales    (502) staff       (20)      114 2024-04-06 15:20:56.000000 geoglows-1.0.0rc2/geoglows/_constants.py
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.751899 geoglows-1.0.0rc2/geoglows/_plots/
--rw-r--r--   0 rchales    (502) staff       (20)       36 2024-03-29 16:40:36.000000 geoglows-1.0.0rc2/geoglows/_plots/__init__.py
--rw-r--r--   0 rchales    (502) staff       (20)      814 2024-03-29 16:40:36.000000 geoglows-1.0.0rc2/geoglows/_plots/format_tools.py
--rw-r--r--   0 rchales    (502) staff       (20)    16451 2024-03-29 16:40:36.000000 geoglows-1.0.0rc2/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 rchales    (502) staff       (20)    11414 2024-04-06 15:20:56.000000 geoglows-1.0.0rc2/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 rchales    (502) staff       (20)     1678 2024-04-06 15:20:56.000000 geoglows-1.0.0rc2/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 rchales    (502) staff       (20)    11477 2024-04-02 00:15:15.000000 geoglows-1.0.0rc2/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 rchales    (502) staff       (20)     6469 2024-04-02 00:15:15.000000 geoglows-1.0.0rc2/geoglows/_plots/plots.py
--rw-r--r--   0 rchales    (502) staff       (20)     7855 2024-04-06 16:33:31.000000 geoglows-1.0.0rc2/geoglows/analyze.py
--rw-r--r--   0 rchales    (502) staff       (20)     8175 2024-03-29 16:40:36.000000 geoglows-1.0.0rc2/geoglows/bias.py
--rw-r--r--   0 rchales    (502) staff       (20)    13163 2024-04-06 17:38:34.000000 geoglows-1.0.0rc2/geoglows/data.py
--rw-r--r--   0 rchales    (502) staff       (20)      801 2024-04-02 00:15:15.000000 geoglows-1.0.0rc2/geoglows/streams.py
--rw-r--r--   0 rchales    (502) staff       (20)     3815 2024-04-06 15:39:50.000000 geoglows-1.0.0rc2/geoglows/tables.py
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.752284 geoglows-1.0.0rc2/geoglows.egg-info/
--rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 17:39:10.000000 geoglows-1.0.0rc2/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 rchales    (502) staff       (20)      981 2024-04-06 17:39:10.000000 geoglows-1.0.0rc2/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 rchales    (502) staff       (20)        1 2024-04-06 17:39:10.000000 geoglows-1.0.0rc2/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 rchales    (502) staff       (20)      109 2024-04-06 17:39:10.000000 geoglows-1.0.0rc2/geoglows.egg-info/requires.txt
--rw-r--r--   0 rchales    (502) staff       (20)        9 2024-04-06 17:39:10.000000 geoglows-1.0.0rc2/geoglows.egg-info/top_level.txt
--rw-r--r--   0 rchales    (502) staff       (20)      108 2024-04-06 15:20:56.000000 geoglows-1.0.0rc2/requirements.txt
--rw-r--r--   0 rchales    (502) staff       (20)       38 2024-04-06 17:39:10.752917 geoglows-1.0.0rc2/setup.cfg
--rw-r--r--   0 rchales    (502) staff       (20)     1653 2024-04-06 16:05:51.000000 geoglows-1.0.0rc2/setup.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.924644 geoglows-1.0.0rc3/
+-rw-r--r--   0 rchales    (502) staff       (20)       98 2024-04-02 00:15:15.000000 geoglows-1.0.0rc3/.gitignore
+-rw-r--r--   0 rchales    (502) staff       (20)      568 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/.readthedocs.yml
+-rw-r--r--   0 rchales    (502) staff       (20)     1519 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/LICENSE
+-rw-r--r--   0 rchales    (502) staff       (20)      173 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/MANIFEST.in
+-rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 18:46:02.924403 geoglows-1.0.0rc3/PKG-INFO
+-rw-r--r--   0 rchales    (502) staff       (20)      780 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/README.md
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.920668 geoglows-1.0.0rc3/docs/
+-rw-r--r--   0 rchales    (502) staff       (20)      634 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/Makefile
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.920775 geoglows-1.0.0rc3/docs/_static/
+-rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/_static/.gitkeep
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.920865 geoglows-1.0.0rc3/docs/_templates/
+-rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/_templates/.gitkeep
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.921378 geoglows-1.0.0rc3/docs/api-documentation/
+-rw-r--r--   0 rchales    (502) staff       (20)      321 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation/analysis.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      210 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation/bias.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      153 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation/examples.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      687 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation/plots.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1241 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation/streamflow.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      791 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1905 2024-03-29 16:40:36.000000 geoglows-1.0.0rc3/docs/conf.py
+-rw-r--r--   0 rchales    (502) staff       (20)      871 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/dev-notes.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     2028 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/index.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1536 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/license.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      100 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/requirements.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      243 2024-04-02 00:15:15.000000 geoglows-1.0.0rc3/environment.yaml
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.922252 geoglows-1.0.0rc3/geoglows/
+-rw-r--r--   0 rchales    (502) staff       (20)      418 2024-04-06 18:29:14.000000 geoglows-1.0.0rc3/geoglows/__init__.py
+-rw-r--r--   0 rchales    (502) staff       (20)      114 2024-04-06 15:20:56.000000 geoglows-1.0.0rc3/geoglows/_constants.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.923733 geoglows-1.0.0rc3/geoglows/_plots/
+-rw-r--r--   0 rchales    (502) staff       (20)       36 2024-03-29 16:40:36.000000 geoglows-1.0.0rc3/geoglows/_plots/__init__.py
+-rw-r--r--   0 rchales    (502) staff       (20)      814 2024-03-29 16:40:36.000000 geoglows-1.0.0rc3/geoglows/_plots/format_tools.py
+-rw-r--r--   0 rchales    (502) staff       (20)    16451 2024-03-29 16:40:36.000000 geoglows-1.0.0rc3/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11414 2024-04-06 15:20:56.000000 geoglows-1.0.0rc3/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 rchales    (502) staff       (20)     1678 2024-04-06 15:20:56.000000 geoglows-1.0.0rc3/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11477 2024-04-02 00:15:15.000000 geoglows-1.0.0rc3/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 rchales    (502) staff       (20)     6469 2024-04-02 00:15:15.000000 geoglows-1.0.0rc3/geoglows/_plots/plots.py
+-rw-r--r--   0 rchales    (502) staff       (20)     7935 2024-04-06 18:29:07.000000 geoglows-1.0.0rc3/geoglows/analyze.py
+-rw-r--r--   0 rchales    (502) staff       (20)     8175 2024-03-29 16:40:36.000000 geoglows-1.0.0rc3/geoglows/bias.py
+-rw-r--r--   0 rchales    (502) staff       (20)    13298 2024-04-06 18:27:49.000000 geoglows-1.0.0rc3/geoglows/data.py
+-rw-r--r--   0 rchales    (502) staff       (20)      801 2024-04-02 00:15:15.000000 geoglows-1.0.0rc3/geoglows/streams.py
+-rw-r--r--   0 rchales    (502) staff       (20)     3815 2024-04-06 15:39:50.000000 geoglows-1.0.0rc3/geoglows/tables.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.924174 geoglows-1.0.0rc3/geoglows.egg-info/
+-rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 18:46:02.000000 geoglows-1.0.0rc3/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 rchales    (502) staff       (20)      981 2024-04-06 18:46:02.000000 geoglows-1.0.0rc3/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 rchales    (502) staff       (20)        1 2024-04-06 18:46:02.000000 geoglows-1.0.0rc3/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      109 2024-04-06 18:46:02.000000 geoglows-1.0.0rc3/geoglows.egg-info/requires.txt
+-rw-r--r--   0 rchales    (502) staff       (20)        9 2024-04-06 18:46:02.000000 geoglows-1.0.0rc3/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      108 2024-04-06 15:20:56.000000 geoglows-1.0.0rc3/requirements.txt
+-rw-r--r--   0 rchales    (502) staff       (20)       38 2024-04-06 18:46:02.924679 geoglows-1.0.0rc3/setup.cfg
+-rw-r--r--   0 rchales    (502) staff       (20)     1653 2024-04-06 16:05:51.000000 geoglows-1.0.0rc3/setup.py
```

### Comparing `geoglows-1.0.0rc2/.readthedocs.yml` & `geoglows-1.0.0rc3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/LICENSE` & `geoglows-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/PKG-INFO` & `geoglows-1.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Package for accessing data from the GEOGloWS V2 Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.0rc2/README.md` & `geoglows-1.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/docs/Makefile` & `geoglows-1.0.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/docs/api-documentation/plots.rst` & `geoglows-1.0.0rc3/docs/api-documentation/plots.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/docs/api-documentation/streamflow.rst` & `geoglows-1.0.0rc3/docs/api-documentation/streamflow.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/docs/api-documentation.rst` & `geoglows-1.0.0rc3/docs/api-documentation.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/docs/conf.py` & `geoglows-1.0.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/docs/dev-notes.rst` & `geoglows-1.0.0rc3/docs/dev-notes.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/docs/index.rst` & `geoglows-1.0.0rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/docs/license.rst` & `geoglows-1.0.0rc3/docs/license.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/geoglows/_plots/format_tools.py` & `geoglows-1.0.0rc3/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.0.0rc3/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.0.0rc3/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/geoglows/_plots/plotly_helpers.py` & `geoglows-1.0.0rc3/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.0.0rc3/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/geoglows/_plots/plots.py` & `geoglows-1.0.0rc3/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/geoglows/analyze.py` & `geoglows-1.0.0rc3/geoglows/analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,16 @@
 
     Args:
         df: a dataframe of retrospective simulation data
 
     Returns:
         pandas DataFrame with an index of "%Y" values for each year
     """
-    return df.groupby(df.index.strftime('%Y')).mean()
+    # select years with >= 365 entries
+    return df.groupby(df.index.strftime('%Y')).filter(lambda x: len(x) >= 365).mean()
 
 
 def daily_variance(df: pd.DataFrame) -> pd.DataFrame:
     """
     Calculate the daily standard deviation of a dataframe with a datetime index
 
     Args:
@@ -154,15 +155,16 @@
       df: historical data to compute daily statistics from
 
     Return:
       pd.DataFrame: dataframe with average, min, 25% values, median, 75% value and max value for each day of year
     """
     daily_grouped = df.groupby(df.index.strftime('%m/%d'))
     return (
-        daily_grouped.mean()
+        daily_grouped
+        .mean()
         .merge(daily_grouped.min(), left_index=True, right_index=True, suffixes=('_avg', '_min'))
         .merge(daily_grouped.quantile(.25), left_index=True, right_index=True)
         .merge(daily_grouped.median(), left_index=True, right_index=True, suffixes=('_25%', '_med'))
         .merge(daily_grouped.quantile(.75), left_index=True, right_index=True)
         .merge(daily_grouped.max(), left_index=True, right_index=True, suffixes=('_75%', '_max'))
     )
```

### Comparing `geoglows-1.0.0rc2/geoglows/bias.py` & `geoglows-1.0.0rc3/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/geoglows/data.py` & `geoglows-1.0.0rc3/geoglows/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 
 import pandas as pd
 import requests
 import s3fs
 import xarray as xr
 
 from ._constants import METADATA_TABLE_LOCAL_PATH
-from .analyze import forecast_stats as calc_forecast_stats, simple_forecast as calc_simple_forecast
+from .analyze import (
+    simple_forecast as calc_simple_forecast,
+    forecast_stats as calc_forecast_stats,
+    daily_averages as calc_daily_averages,
+    monthly_averages as calc_monthly_averages,
+    annual_averages as calc_annual_averages,
+)
 
 __all__ = [
     'dates',
     'forecast',
     'forecast_stats',
     'forecast_ensembles',
     'forecast_records',
@@ -37,33 +43,33 @@
 def _forecast_endpoint_decorator(function):
     def from_aws(*args, **kwargs):
         product_name = function.__name__.replace("_", "").lower()
         if product_name == 'forecastrecords':
             warnings.warn('forecast_records are not available from the AWS Open Data Program.')
             return from_rest(*args, **kwargs)
 
+        reach_id = args[0] if len(args) > 0 else None
+        reach_id = kwargs.get('reach_id', '') if not reach_id else reach_id
+
         s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
-        date = kwargs.get('date', '')
-        if date is not None and not product_name == 'dates':
+        if kwargs.get('date', '') and not product_name == 'dates':
+            date = kwargs['date']
             if len(date) == 8:
                 date = f'{date}00.zarr'
             elif len(date) == 10:
                 date = f'{date}.zarr'
             else:
                 raise ValueError('Date must be YYYYMMDD or YYYYMMDDHH format. Use dates() to view available data.')
         else:
             dates = sorted([x.split('/')[-1] for x in s3.ls(ODP_FORECAST_S3_BUCKET_URI)])
             if product_name == 'dates':
                 return dates
             date = dates[-1]
         s3store = s3fs.S3Map(root=f'{ODP_FORECAST_S3_BUCKET_URI}/{date}', s3=s3, check=False)
 
-        reach_id = args[0] if len(args) > 0 else None
-        reach_id = kwargs.get('reach_id', '') if not reach_id else reach_id
-
         df = xr.open_zarr(s3store).sel(rivid=reach_id).to_dataframe().round(2).reset_index()
 
         # rename columns to match the REST API
         if type(reach_id) is list:
             df = df.pivot(columns='ensemble', index=['time', 'rivid'], values='Qout')
         else:
             df = df.pivot(index='time', columns='ensemble', values='Qout')
@@ -141,15 +147,18 @@
             return response.json()
         else:
             raise ValueError(f'Unsupported return format requested: {return_format}')
 
     def main(*args, **kwargs):
         source = kwargs.get('data_source', 'rest')
         assert source in ('rest', 'aws'), ValueError(f'Unrecognized data source requested: {source}')
-        return from_rest(*args, **kwargs) if source == 'rest' else from_aws(*args, **kwargs)
+        if source == 'rest':
+            return from_rest(*args, **kwargs)
+        else:
+            return from_aws(*args, **kwargs)
 
     return main
 
 
 # Forecast data and derived products
 @_forecast_endpoint_decorator
 def dates(**kwargs) -> dict or str:
@@ -268,43 +277,43 @@
     Args:
         reach_id: the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
     df = retrospective(reach_id)
-    return df.groupby(df.index.strftime('%m%d')).mean()
+    return calc_daily_averages(df)
 
 
 def monthly_averages(reach_id: int or list) -> pd.DataFrame:
     """
     Retrieves monthly average streamflow for a given reach_id
 
     Args:
         reach_id: the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
     df = retrospective(reach_id)
-    return df.groupby(df.index.strftime('%m')).mean()
+    return calc_monthly_averages(df)
 
 
 def annual_averages(reach_id: int or list) -> pd.DataFrame:
     """
     Retrieves annual average streamflow for a given reach_id
 
     Args:
         reach_id: the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
     df = retrospective(reach_id)
-    return df.groupby(df.index.strftime('%Y')).mean()
+    return calc_annual_averages(df)
 
 
 def return_periods(reach_id: int or list) -> pd.DataFrame:
     """
     Retrieves the return period thresholds based on a specified historic simulation forcing on a certain reach_id.
 
     Args:
```

### Comparing `geoglows-1.0.0rc2/geoglows/streams.py` & `geoglows-1.0.0rc3/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/geoglows/tables.py` & `geoglows-1.0.0rc3/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/geoglows.egg-info/PKG-INFO` & `geoglows-1.0.0rc3/geoglows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Package for accessing data from the GEOGloWS V2 Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.0rc2/geoglows.egg-info/SOURCES.txt` & `geoglows-1.0.0rc3/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc2/setup.py` & `geoglows-1.0.0rc3/setup.py`

 * *Files identical despite different names*

