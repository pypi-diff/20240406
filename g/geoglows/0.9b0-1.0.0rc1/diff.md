# Comparing `tmp/geoglows-0.9b0.tar.gz` & `tmp/geoglows-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geoglows-0.9b0.tar", last modified: Fri Nov 15 22:09:30 2019, max compression
+gzip compressed data, was "geoglows-1.0.0rc1.tar", last modified: Sat Apr  6 16:00:18 2024, max compression
```

## Comparing `geoglows-0.9b0.tar` & `geoglows-1.0.0rc1.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/
--rw-r--r--   0 rileyhales   (503) staff       (20)      149 2019-11-15 05:02:51.000000 geoglows-0.9b0/MANIFEST.in
--rw-r--r--   0 rileyhales   (503) staff       (20)     1714 2019-11-15 22:09:30.000000 geoglows-0.9b0/PKG-INFO
--rw-r--r--   0 rileyhales   (503) staff       (20)     1108 2019-11-08 00:27:59.000000 geoglows-0.9b0/README.md
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/
--rw-r--r--   0 rileyhales   (503) staff       (20)       69 2019-10-26 03:44:47.000000 geoglows-0.9b0/geoglows/__init__.py
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/africa-geoglows/
--rwxr-xr-x   0 rileyhales   (503) staff       (20)  3442076 2019-11-15 03:53:04.000000 geoglows-0.9b0/geoglows/delineation_data/africa-geoglows/comid_lat_lon_z.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/australia-geoglows/
--rwxr-xr-x   0 rileyhales   (503) staff       (20)  2000629 2019-11-15 03:53:04.000000 geoglows-0.9b0/geoglows/delineation_data/australia-geoglows/comid_lat_lon_z.csv
--rw-r--r--   0 rileyhales   (503) staff       (20)      475 2019-11-15 03:53:04.000000 geoglows-0.9b0/geoglows/delineation_data/bounding_boxes.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/central_america-geoglows/
--rwxr-xr-x   0 rileyhales   (503) staff       (20)  1758881 2019-11-15 03:53:04.000000 geoglows-0.9b0/geoglows/delineation_data/central_america-geoglows/comid_lat_lon_z.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/central_asia-geoglows/
--rw-r--r--   0 rileyhales   (503) staff       (20)  1766227 2019-11-15 03:53:04.000000 geoglows-0.9b0/geoglows/delineation_data/central_asia-geoglows/comid_lat_lon_z.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/east_asia-geoglows/
--rw-r--r--   0 rileyhales   (503) staff       (20)  2538302 2019-11-15 03:53:05.000000 geoglows-0.9b0/geoglows/delineation_data/east_asia-geoglows/comid_lat_lon_z.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/europe-geoglows/
--rw-r--r--   0 rileyhales   (503) staff       (20)  2658162 2019-11-15 03:53:05.000000 geoglows-0.9b0/geoglows/delineation_data/europe-geoglows/comid_lat_lon_z.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/indonesia-geoglows/
--rw-r--r--   0 rileyhales   (503) staff       (20)  1035584 2019-11-15 03:53:05.000000 geoglows-0.9b0/geoglows/delineation_data/indonesia-geoglows/comid_lat_lon_z.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/japan-geoglows/
--rw-r--r--   0 rileyhales   (503) staff       (20)   258549 2019-11-15 03:53:05.000000 geoglows-0.9b0/geoglows/delineation_data/japan-geoglows/comid_lat_lon_z.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/middle_east-geoglows/
--rwxr-xr-x   0 rileyhales   (503) staff       (20)  1263224 2019-11-15 03:53:05.000000 geoglows-0.9b0/geoglows/delineation_data/middle_east-geoglows/comid_lat_lon_z.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/northamerica-geoglows/
--rw-r--r--   0 rileyhales   (503) staff       (20)  1381003 2019-11-15 03:53:05.000000 geoglows-0.9b0/geoglows/delineation_data/northamerica-geoglows/comid_lat_lon_z.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/south_america-geoglows/
--rwxr-xr-x   0 rileyhales   (503) staff       (20)  5022675 2019-11-15 03:53:05.000000 geoglows-0.9b0/geoglows/delineation_data/south_america-geoglows/comid_lat_lon_z.csv
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/delineation_data/south_asia-geoglows/
--rwxr-xr-x   0 rileyhales   (503) staff       (20)  2669741 2019-11-15 03:53:05.000000 geoglows-0.9b0/geoglows/delineation_data/south_asia-geoglows/comid_lat_lon_z.csv
--rw-r--r--   0 rileyhales   (503) staff       (20)     1736 2019-11-08 00:27:59.000000 geoglows-0.9b0/geoglows/gfs.py
--rw-r--r--   0 rileyhales   (503) staff       (20)     1474 2019-10-25 23:18:47.000000 geoglows-0.9b0/geoglows/gldas.py
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/notebooks/
--rw-r--r--   0 rileyhales   (503) staff       (20)     8448 2019-11-15 05:01:04.000000 geoglows-0.9b0/geoglows/notebooks/GEOGloWS_ECMWF_Streamflow_Interaction.ipynb
--rw-r--r--   0 rileyhales   (503) staff       (20)     3310 2019-11-08 00:27:59.000000 geoglows-0.9b0/geoglows/notebooks/gfs.ipynb
--rw-r--r--   0 rileyhales   (503) staff       (20)     3189 2019-11-08 00:27:59.000000 geoglows-0.9b0/geoglows/notebooks/gldas.ipynb
--rw-r--r--   0 rileyhales   (503) staff       (20)    27178 2019-11-15 20:54:42.000000 geoglows-0.9b0/geoglows/streamflow.py
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows/templates/
--rw-r--r--   0 rileyhales   (503) staff       (20)     1118 2019-11-15 03:53:05.000000 geoglows-0.9b0/geoglows/templates/probabilities_table.html
-drwxr-xr-x   0 rileyhales   (503) staff       (20)        0 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows.egg-info/
--rw-r--r--   0 rileyhales   (503) staff       (20)     1714 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 rileyhales   (503) staff       (20)     1268 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 rileyhales   (503) staff       (20)        1 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 rileyhales   (503) staff       (20)       44 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows.egg-info/requires.txt
--rw-r--r--   0 rileyhales   (503) staff       (20)        9 2019-11-15 22:09:30.000000 geoglows-0.9b0/geoglows.egg-info/top_level.txt
--rw-r--r--   0 rileyhales   (503) staff       (20)       38 2019-11-15 22:09:30.000000 geoglows-0.9b0/setup.cfg
--rw-r--r--   0 rileyhales   (503) staff       (20)      789 2019-11-15 21:08:23.000000 geoglows-0.9b0/setup.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.124338 geoglows-1.0.0rc1/
+-rw-r--r--   0 rchales    (502) staff       (20)       98 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/.gitignore
+-rw-r--r--   0 rchales    (502) staff       (20)      568 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/.readthedocs.yml
+-rw-r--r--   0 rchales    (502) staff       (20)     1519 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/LICENSE
+-rw-r--r--   0 rchales    (502) staff       (20)      173 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 16:00:18.124141 geoglows-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 rchales    (502) staff       (20)      780 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/README.md
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.120281 geoglows-1.0.0rc1/docs/
+-rw-r--r--   0 rchales    (502) staff       (20)      634 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/Makefile
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.120430 geoglows-1.0.0rc1/docs/_static/
+-rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/_static/.gitkeep
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.120549 geoglows-1.0.0rc1/docs/_templates/
+-rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/_templates/.gitkeep
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.121153 geoglows-1.0.0rc1/docs/api-documentation/
+-rw-r--r--   0 rchales    (502) staff       (20)      321 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation/analysis.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      210 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation/bias.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      153 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation/examples.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      687 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation/plots.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1241 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation/streamflow.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      791 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/api-documentation.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1905 2024-03-29 16:40:36.000000 geoglows-1.0.0rc1/docs/conf.py
+-rw-r--r--   0 rchales    (502) staff       (20)      871 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/dev-notes.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     2028 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/index.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1536 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/license.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      100 2024-03-29 16:38:01.000000 geoglows-1.0.0rc1/docs/requirements.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      243 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/environment.yaml
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.122000 geoglows-1.0.0rc1/geoglows/
+-rw-r--r--   0 rchales    (502) staff       (20)      418 2024-04-06 15:58:46.000000 geoglows-1.0.0rc1/geoglows/__init__.py
+-rw-r--r--   0 rchales    (502) staff       (20)      114 2024-04-06 15:20:56.000000 geoglows-1.0.0rc1/geoglows/_constants.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.123421 geoglows-1.0.0rc1/geoglows/_plots/
+-rw-r--r--   0 rchales    (502) staff       (20)       36 2024-03-29 16:40:36.000000 geoglows-1.0.0rc1/geoglows/_plots/__init__.py
+-rw-r--r--   0 rchales    (502) staff       (20)      814 2024-03-29 16:40:36.000000 geoglows-1.0.0rc1/geoglows/_plots/format_tools.py
+-rw-r--r--   0 rchales    (502) staff       (20)    16451 2024-03-29 16:40:36.000000 geoglows-1.0.0rc1/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11414 2024-04-06 15:20:56.000000 geoglows-1.0.0rc1/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 rchales    (502) staff       (20)     1678 2024-04-06 15:20:56.000000 geoglows-1.0.0rc1/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11477 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 rchales    (502) staff       (20)     6469 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/geoglows/_plots/plots.py
+-rw-r--r--   0 rchales    (502) staff       (20)     6735 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/geoglows/analyze.py
+-rw-r--r--   0 rchales    (502) staff       (20)     8175 2024-03-29 16:40:36.000000 geoglows-1.0.0rc1/geoglows/bias.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11070 2024-04-06 15:20:56.000000 geoglows-1.0.0rc1/geoglows/data.py
+-rw-r--r--   0 rchales    (502) staff       (20)      801 2024-04-02 00:15:15.000000 geoglows-1.0.0rc1/geoglows/streams.py
+-rw-r--r--   0 rchales    (502) staff       (20)     3815 2024-04-06 15:39:50.000000 geoglows-1.0.0rc1/geoglows/tables.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 16:00:18.123901 geoglows-1.0.0rc1/geoglows.egg-info/
+-rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 16:00:18.000000 geoglows-1.0.0rc1/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 rchales    (502) staff       (20)      981 2024-04-06 16:00:18.000000 geoglows-1.0.0rc1/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 rchales    (502) staff       (20)        1 2024-04-06 16:00:18.000000 geoglows-1.0.0rc1/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      109 2024-04-06 16:00:18.000000 geoglows-1.0.0rc1/geoglows.egg-info/requires.txt
+-rw-r--r--   0 rchales    (502) staff       (20)        9 2024-04-06 16:00:18.000000 geoglows-1.0.0rc1/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      108 2024-04-06 15:20:56.000000 geoglows-1.0.0rc1/requirements.txt
+-rw-r--r--   0 rchales    (502) staff       (20)       38 2024-04-06 16:00:18.124376 geoglows-1.0.0rc1/setup.cfg
+-rw-r--r--   0 rchales    (502) staff       (20)     1806 2024-04-06 16:00:17.000000 geoglows-1.0.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

