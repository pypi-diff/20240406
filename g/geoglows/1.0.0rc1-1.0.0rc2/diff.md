# Comparing `tmp/geoglows-1.0.0rc1.tar.gz` & `tmp/geoglows-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.0.0rc1.tar", last modified: Sat Apr  6 16:00:18 2024, max compression
+gzip compressed data, was "geoglows-1.0.0rc2.tar", last modified: Sat Apr  6 17:39:10 2024, max compression
```

## Comparing `geoglows-1.0.0rc1.tar` & `geoglows-1.0.0rc2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.124338 geoglows-1.0.0rc1/
--rw-r--r--   0 rchales    (502) staff       (20)       98 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/.gitignore
--rw-r--r--   0 rchales    (502) staff       (20)      568 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/.readthedocs.yml
--rw-r--r--   0 rchales    (502) staff       (20)     1519 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/LICENSE
--rw-r--r--   0 rchales    (502) staff       (20)      173 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 16:00:18.124141 geoglows-1.0.0rc1/PKG-INFO
--rw-r--r--   0 rchales    (502) staff       (20)      780 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/README.md
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.120281 geoglows-1.0.0rc1/docs/
--rw-r--r--   0 rchales    (502) staff       (20)      634 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/Makefile
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.120430 geoglows-1.0.0rc1/docs/_static/
--rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/_static/.gitkeep
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.120549 geoglows-1.0.0rc1/docs/_templates/
--rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/_templates/.gitkeep
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.121153 geoglows-1.0.0rc1/docs/api-documentation/
--rw-r--r--   0 rchales    (502) staff       (20)      321 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation/analysis.rst
--rw-r--r--   0 rchales    (502) staff       (20)      210 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation/bias.rst
--rw-r--r--   0 rchales    (502) staff       (20)      153 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation/examples.rst
--rw-r--r--   0 rchales    (502) staff       (20)      687 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation/plots.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1241 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation/streamflow.rst
--rw-r--r--   0 rchales    (502) staff       (20)      791 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1905 2024-03-29 16:40:36.000000 geoglows-1.0.0rc1/docs/conf.py
--rw-r--r--   0 rchales    (502) staff       (20)      871 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/dev-notes.rst
--rw-r--r--   0 rchales    (502) staff       (20)     2028 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/index.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1536 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/license.rst
--rw-r--r--   0 rchales    (502) staff       (20)      100 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/requirements.txt
--rw-r--r--   0 rchales    (502) staff       (20)      243 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/environment.yaml
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.122000 geoglows-1.0.0rc1/geoglows/
--rw-r--r--   0 rchales    (502) staff       (20)      418 2024-04-06 15:58:46.000000 geoglows-1.0.0rc1/geoglows/__init__.py
--rw-r--r--   0 rchales    (502) staff       (20)      114 2024-04-06 15:20:56.000000 geoglows-1.0.0rc1/geoglows/_constants.py
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.123421 geoglows-1.0.0rc1/geoglows/_plots/
--rw-r--r--   0 rchales    (502) staff       (20)       36 2024-03-29 16:40:36.000000 geoglows-1.0.0rc1/geoglows/_plots/__init__.py
--rw-r--r--   0 rchales    (502) staff       (20)      814 2024-03-29 16:40:36.000000 geoglows-1.0.0rc1/geoglows/_plots/format_tools.py
--rw-r--r--   0 rchales    (502) staff       (20)    16451 2024-03-29 16:40:36.000000 geoglows-1.0.0rc1/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 rchales    (502) staff       (20)    11414 2024-04-06 15:20:56.000000 geoglows-1.0.0rc1/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 rchales    (502) staff       (20)     1678 2024-04-06 15:20:56.000000 geoglows-1.0.0rc1/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 rchales    (502) staff       (20)    11477 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 rchales    (502) staff       (20)     6469 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/geoglows/_plots/plots.py
--rw-r--r--   0 rchales    (502) staff       (20)     6735 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/geoglows/analyze.py
--rw-r--r--   0 rchales    (502) staff       (20)     8175 2024-03-29 16:40:36.000000 geoglows-1.0.0rc1/geoglows/bias.py
--rw-r--r--   0 rchales    (502) staff       (20)    11070 2024-04-06 15:20:56.000000 geoglows-1.0.0rc1/geoglows/data.py
--rw-r--r--   0 rchales    (502) staff       (20)      801 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/geoglows/streams.py
--rw-r--r--   0 rchales    (502) staff       (20)     3815 2024-04-06 15:39:50.000000 geoglows-1.0.0rc1/geoglows/tables.py
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.123901 geoglows-1.0.0rc1/geoglows.egg-info/
--rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 16:00:18.000000 geoglows-1.0.0rc1/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 rchales    (502) staff       (20)      981 2024-04-06 16:00:18.000000 geoglows-1.0.0rc1/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 rchales    (502) staff       (20)        1 2024-04-06 16:00:18.000000 geoglows-1.0.0rc1/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 rchales    (502) staff       (20)      109 2024-04-06 16:00:18.000000 geoglows-1.0.0rc1/geoglows.egg-info/requires.txt
--rw-r--r--   0 rchales    (502) staff       (20)        9 2024-04-06 16:00:18.000000 geoglows-1.0.0rc1/geoglows.egg-info/top_level.txt
--rw-r--r--   0 rchales    (502) staff       (20)      108 2024-04-06 15:20:56.000000 geoglows-1.0.0rc1/requirements.txt
--rw-r--r--   0 rchales    (502) staff       (20)       38 2024-04-06 16:00:18.124376 geoglows-1.0.0rc1/setup.cfg
--rw-r--r--   0 rchales    (502) staff       (20)     1806 2024-04-06 16:00:17.000000 geoglows-1.0.0rc1/setup.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.752873 geoglows-1.0.0rc2/
+-rw-r--r--   0 rchales    (502) staff       (20)       98 2024-04-02 00:15:15.000000 geoglows-1.0.0rc2/.gitignore
+-rw-r--r--   0 rchales    (502) staff       (20)      568 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/.readthedocs.yml
+-rw-r--r--   0 rchales    (502) staff       (20)     1519 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/LICENSE
+-rw-r--r--   0 rchales    (502) staff       (20)      173 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/MANIFEST.in
+-rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 17:39:10.752566 geoglows-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 rchales    (502) staff       (20)      780 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/README.md
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.743621 geoglows-1.0.0rc2/docs/
+-rw-r--r--   0 rchales    (502) staff       (20)      634 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/Makefile
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.743732 geoglows-1.0.0rc2/docs/_static/
+-rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/_static/.gitkeep
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.743828 geoglows-1.0.0rc2/docs/_templates/
+-rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/_templates/.gitkeep
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.744400 geoglows-1.0.0rc2/docs/api-documentation/
+-rw-r--r--   0 rchales    (502) staff       (20)      321 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation/analysis.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      210 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation/bias.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      153 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation/examples.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      687 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation/plots.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1241 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation/streamflow.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      791 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/api-documentation.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1905 2024-03-29 16:40:36.000000 geoglows-1.0.0rc2/docs/conf.py
+-rw-r--r--   0 rchales    (502) staff       (20)      871 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/dev-notes.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     2028 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/index.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1536 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/license.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      100 2024-03-29 16:38:01.000000 geoglows-1.0.0rc2/docs/requirements.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      243 2024-04-02 00:15:15.000000 geoglows-1.0.0rc2/environment.yaml
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.745352 geoglows-1.0.0rc2/geoglows/
+-rw-r--r--   0 rchales    (502) staff       (20)      418 2024-04-06 17:38:45.000000 geoglows-1.0.0rc2/geoglows/__init__.py
+-rw-r--r--   0 rchales    (502) staff       (20)      114 2024-04-06 15:20:56.000000 geoglows-1.0.0rc2/geoglows/_constants.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.751899 geoglows-1.0.0rc2/geoglows/_plots/
+-rw-r--r--   0 rchales    (502) staff       (20)       36 2024-03-29 16:40:36.000000 geoglows-1.0.0rc2/geoglows/_plots/__init__.py
+-rw-r--r--   0 rchales    (502) staff       (20)      814 2024-03-29 16:40:36.000000 geoglows-1.0.0rc2/geoglows/_plots/format_tools.py
+-rw-r--r--   0 rchales    (502) staff       (20)    16451 2024-03-29 16:40:36.000000 geoglows-1.0.0rc2/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11414 2024-04-06 15:20:56.000000 geoglows-1.0.0rc2/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 rchales    (502) staff       (20)     1678 2024-04-06 15:20:56.000000 geoglows-1.0.0rc2/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11477 2024-04-02 00:15:15.000000 geoglows-1.0.0rc2/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 rchales    (502) staff       (20)     6469 2024-04-02 00:15:15.000000 geoglows-1.0.0rc2/geoglows/_plots/plots.py
+-rw-r--r--   0 rchales    (502) staff       (20)     7855 2024-04-06 16:33:31.000000 geoglows-1.0.0rc2/geoglows/analyze.py
+-rw-r--r--   0 rchales    (502) staff       (20)     8175 2024-03-29 16:40:36.000000 geoglows-1.0.0rc2/geoglows/bias.py
+-rw-r--r--   0 rchales    (502) staff       (20)    13163 2024-04-06 17:38:34.000000 geoglows-1.0.0rc2/geoglows/data.py
+-rw-r--r--   0 rchales    (502) staff       (20)      801 2024-04-02 00:15:15.000000 geoglows-1.0.0rc2/geoglows/streams.py
+-rw-r--r--   0 rchales    (502) staff       (20)     3815 2024-04-06 15:39:50.000000 geoglows-1.0.0rc2/geoglows/tables.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 17:39:10.752284 geoglows-1.0.0rc2/geoglows.egg-info/
+-rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 17:39:10.000000 geoglows-1.0.0rc2/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 rchales    (502) staff       (20)      981 2024-04-06 17:39:10.000000 geoglows-1.0.0rc2/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 rchales    (502) staff       (20)        1 2024-04-06 17:39:10.000000 geoglows-1.0.0rc2/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      109 2024-04-06 17:39:10.000000 geoglows-1.0.0rc2/geoglows.egg-info/requires.txt
+-rw-r--r--   0 rchales    (502) staff       (20)        9 2024-04-06 17:39:10.000000 geoglows-1.0.0rc2/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      108 2024-04-06 15:20:56.000000 geoglows-1.0.0rc2/requirements.txt
+-rw-r--r--   0 rchales    (502) staff       (20)       38 2024-04-06 17:39:10.752917 geoglows-1.0.0rc2/setup.cfg
+-rw-r--r--   0 rchales    (502) staff       (20)     1653 2024-04-06 16:05:51.000000 geoglows-1.0.0rc2/setup.py
```

### Comparing `geoglows-1.0.0rc1/.readthedocs.yml` & `geoglows-1.0.0rc2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/LICENSE` & `geoglows-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/PKG-INFO` & `geoglows-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Package for accessing data from the GEOGloWS V2 Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.0rc1/README.md` & `geoglows-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/docs/Makefile` & `geoglows-1.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/docs/api-documentation/plots.rst` & `geoglows-1.0.0rc2/docs/api-documentation/plots.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/docs/api-documentation/streamflow.rst` & `geoglows-1.0.0rc2/docs/api-documentation/streamflow.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/docs/api-documentation.rst` & `geoglows-1.0.0rc2/docs/api-documentation.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/docs/conf.py` & `geoglows-1.0.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/docs/dev-notes.rst` & `geoglows-1.0.0rc2/docs/dev-notes.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/docs/index.rst` & `geoglows-1.0.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/docs/license.rst` & `geoglows-1.0.0rc2/docs/license.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/geoglows/_plots/format_tools.py` & `geoglows-1.0.0rc2/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.0.0rc2/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.0.0rc2/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/geoglows/_plots/plotly_helpers.py` & `geoglows-1.0.0rc2/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.0.0rc2/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/geoglows/_plots/plots.py` & `geoglows-1.0.0rc2/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/geoglows/analyze.py` & `geoglows-1.0.0rc2/geoglows/analyze.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import math
 
 import numpy as np
 import pandas as pd
 
 __all__ = [
     'gumbel1',
+    'simple_forecast',
+    'forecast_stats',
     'daily_averages',
     'monthly_averages',
     'annual_averages',
     'daily_stats',
     'daily_variance',
     'daily_flow_anomaly',
     'return_periods',
@@ -49,14 +51,53 @@
         f'flow_uncertainty_upper_cms': np.nanpercentile(df.values, 80, axis=1),
         f'flow_median_cms': np.median(df.values, axis=1),
         f'flow_uncertainty_lower_cms': np.nanpercentile(df.values, 20, axis=1),
     }, index=df.index)
     return df
 
 
+def forecast_stats(ens: pd.DataFrame) -> pd.DataFrame:
+    """
+    Calculates the statistics for a dataframe of forecast ensembles
+
+    Args:
+        ens: a dataframe of forecast ensembles
+
+    Returns:
+        pandas DataFrame with an index of datetime and columns min, max, mean, median, 25%, 75%
+    """
+    df = (
+        ens
+        .drop(columns=['ensemble_52_cms'])
+        .dropna()
+    )
+    return (
+        pd
+        .DataFrame(
+            {
+                'flow_min_cms': df.min(axis=1),
+                'flow_25p_cms': df.quantile(.25, axis=1),
+                'flow_avg_cms': df.mean(axis=1),
+                'flow_med_cms': df.median(axis=1),
+                'flow_75p_cms': df.quantile(.75, axis=1),
+                'flow_max_cms': df.max(axis=1),
+            },
+            index=df.index
+        )
+        .merge(
+            ens[['ensemble_52_cms']]
+            .rename(columns={'ensemble_52_cms': 'high_res_cms'}),
+            left_index=True,
+            right_index=True,
+            how='outer'
+        )
+        .sort_index(ascending=True)
+    )
+
+
 def daily_averages(df: pd.DataFrame) -> pd.DataFrame:
     """
     Calculates the daily average of a dataframe with a datetime index
 
     Args:
         df: a dataframe of retrospective simulation data
```

### Comparing `geoglows-1.0.0rc1/geoglows/bias.py` & `geoglows-1.0.0rc2/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/geoglows/data.py` & `geoglows-1.0.0rc2/geoglows/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pandas as pd
 import requests
 import s3fs
 import xarray as xr
 
 from ._constants import METADATA_TABLE_LOCAL_PATH
+from .analyze import forecast_stats as calc_forecast_stats, simple_forecast as calc_simple_forecast
 
 __all__ = [
     'dates',
     'forecast',
     'forecast_stats',
     'forecast_ensembles',
     'forecast_records',
@@ -24,20 +25,64 @@
 
     'metadata_tables',
 ]
 
 DEFAULT_REST_ENDPOINT = 'https://geoglows.ecmwf.int/api/'
 DEFAULT_REST_ENDPOINT_VERSION = 'v2'  # 'v1, v2, latest'
 ODP_CORE_S3_BUCKET_URI = 's3://geoglows-v2'
+ODP_FORECAST_S3_BUCKET_URI = 's3://geoglows-v2-forecasts'
 ODP_RETROSPECTIVE_S3_BUCKET_URI = 's3://geoglows-v2-retrospective'
 ODP_S3_BUCKET_REGION = 'us-west-2'
 
 
 def _forecast_endpoint_decorator(function):
-    def wrapper(*args, **kwargs):
+    def from_aws(*args, **kwargs):
+        product_name = function.__name__.replace("_", "").lower()
+        if product_name == 'forecastrecords':
+            warnings.warn('forecast_records are not available from the AWS Open Data Program.')
+            return from_rest(*args, **kwargs)
+
+        s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
+        date = kwargs.get('date', '')
+        if date is not None and not product_name == 'dates':
+            if len(date) == 8:
+                date = f'{date}00.zarr'
+            elif len(date) == 10:
+                date = f'{date}.zarr'
+            else:
+                raise ValueError('Date must be YYYYMMDD or YYYYMMDDHH format. Use dates() to view available data.')
+        else:
+            dates = sorted([x.split('/')[-1] for x in s3.ls(ODP_FORECAST_S3_BUCKET_URI)])
+            if product_name == 'dates':
+                return dates
+            date = dates[-1]
+        s3store = s3fs.S3Map(root=f'{ODP_FORECAST_S3_BUCKET_URI}/{date}', s3=s3, check=False)
+
+        reach_id = args[0] if len(args) > 0 else None
+        reach_id = kwargs.get('reach_id', '') if not reach_id else reach_id
+
+        df = xr.open_zarr(s3store).sel(rivid=reach_id).to_dataframe().round(2).reset_index()
+
+        # rename columns to match the REST API
+        if type(reach_id) is list:
+            df = df.pivot(columns='ensemble', index=['time', 'rivid'], values='Qout')
+        else:
+            df = df.pivot(index='time', columns='ensemble', values='Qout')
+        df = df[sorted(df.columns)]
+        df.columns = [f'ensemble_{str(x).zfill(2)}_cms' for x in df.columns]
+
+        if product_name == 'forecastensembles':
+            return df
+        elif product_name == 'forecaststats':
+            return calc_forecast_stats(df)
+        elif product_name == 'forecast':
+            return calc_simple_forecast(df)
+        return
+
+    def from_rest(*args, **kwargs):
         # update the default values set by the function unless the user has already specified them
         for key, value in function.__kwdefaults__.items() if function.__kwdefaults__ else []:
             if key not in kwargs:
                 kwargs[key] = value
 
         return_url = kwargs.get('format', 'csv') == 'url'
 
@@ -93,29 +138,34 @@
                 df = df.set_index('datetime')
             return df
         elif return_format == 'json':
             return response.json()
         else:
             raise ValueError(f'Unsupported return format requested: {return_format}')
 
-    return wrapper
+    def main(*args, **kwargs):
+        source = kwargs.get('data_source', 'rest')
+        assert source in ('rest', 'aws'), ValueError(f'Unrecognized data source requested: {source}')
+        return from_rest(*args, **kwargs) if source == 'rest' else from_aws(*args, **kwargs)
+
+    return main
 
 
 # Forecast data and derived products
 @_forecast_endpoint_decorator
 def dates(**kwargs) -> dict or str:
     """
     Gets a list of available forecast product dates
 
     Keyword Args:
         format: csv, json, or url, default csv
-        endpoint: the endpoint of an api instance, only applicable for package or rest endpoint developers
+        data_source: location to query for data, either 'rest' or 'aws'
 
     Returns:
-        pd.DataFrame or dict
+        dict or str
 
         the csv is a single column with a header of 'available_dates' and 1 row per date, sorted oldest to newest
         The dictionary structure is {'available_dates': ['list', 'of', 'dates', 'YYYYMMDD', 'format']}
     """
     pass
 
 
@@ -124,15 +174,15 @@
     """
     Gets the average forecasted flow for a certain reach_id on a certain date
 
     Keyword Args:
         reach_id: the ID of a stream, should be a 9 digit integer
         date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
         format: csv, json, or url, default csv
-        endpoint: the endpoint of an api instance, only applicable for package or rest endpoint developers
+        data_source: location to query for data, either 'rest' or 'aws'
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
@@ -142,15 +192,15 @@
     Retrieves the min, 25%, mean, median, 75%, and max river discharge of the 51 ensembles members for a reach_id
     The 52nd higher resolution member is excluded
 
     Keyword Args:
         reach_id: the ID of a stream, should be a 9 digit integer
         date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
         format: csv, json, or url, default csv
-        endpoint: the endpoint of an api instance, only applicable for package or rest endpoint developers
+        data_source: location to query for data, either 'rest' or 'aws'
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
@@ -159,15 +209,15 @@
     """
     Retrieves each of 52 time series of forecasted discharge for a reach_id on a certain date
 
     Keyword Args:
         reach_id: the ID of a stream, should be a 9 digit integer
         date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
         format: csv, json, or url, default csv
-        endpoint: the endpoint of an api instance, only applicable for package or rest endpoint developers
+        data_source: location to query for data, either 'rest' or 'aws'
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
@@ -177,19 +227,17 @@
     Retrieves a csv showing the ensemble average forecasted flow for the year from January 1 to the current date
 
     Keyword Args:
         reach_id: the ID of a stream, should be a 9 digit integer
         start_date: a YYYYMMDD string giving the earliest date this year to include, defaults to YYYY0101
         end_date: a YYYYMMDD string giving the latest date this year to include, defaults to latest available
         format: csv, json, or url, default csv
-        endpoint: the endpoint of an api instance, only applicable for package or rest endpoint developers
 
     Returns:
         pd.DataFrame or dict or str
-
     """
     pass
 
 
 # Retrospective simulation and derived products
 def retrospective(reach_id: int or list) -> pd.DataFrame:
     """
```

### Comparing `geoglows-1.0.0rc1/geoglows/streams.py` & `geoglows-1.0.0rc2/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/geoglows/tables.py` & `geoglows-1.0.0rc2/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/geoglows.egg-info/PKG-INFO` & `geoglows-1.0.0rc2/geoglows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Package for accessing data from the GEOGloWS V2 Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.0rc1/geoglows.egg-info/SOURCES.txt` & `geoglows-1.0.0rc2/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc1/setup.py` & `geoglows-1.0.0rc2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 REQUIRES_PYTHON = '>=3.10.0'
 LICENSE = 'BSD 3-Clause Clear License'
 
 with open("README.md", "r") as readme:
     LONG_DESCRIPTION = readme.read()
 
 with open(f'./{NAME}/__init__.py') as f:
-    # version_pattern = r'__version__ = [\'"](\d+\.\d+\.\d+)[\'"]'
-    # make an re string that matches the contents of eveything after '__version__ = '
     version_pattern = r'__version__ = [\'"](.+)[\'"]'
     VERSION = re.search(version_pattern, f.read()).group(1)
 
 with open('./requirements.txt') as f:
     INSTALL_REQUIRES = f.read().splitlines()
 
 setup(
```

