# Comparing `tmp/pygmtsar-2024.3.15.post5.tar.gz` & `tmp/pygmtsar-2024.3.15.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2024.3.15.post5.tar", last modified: Wed Mar 27 12:19:00 2024, max compression
+gzip compressed data, was "pygmtsar-2024.3.15.post7.tar", last modified: Sat Apr  6 16:13:18 2024, max compression
```

## Comparing `pygmtsar-2024.3.15.post5.tar` & `pygmtsar-2024.3.15.post7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-03-27 12:19:00.381827 pygmtsar-2024.3.15.post5/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.3.15.post5/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-03-27 12:19:00.381553 pygmtsar-2024.3.15.post5/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)    11721 2024-03-15 14:17:09.000000 pygmtsar-2024.3.15.post5/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-03-27 12:19:00.380124 pygmtsar-2024.3.15.post5/pygmtsar/
--rw-r--r--   0 mbg        (501) staff       (20)    20813 2024-03-21 13:49:04.000000 pygmtsar-2024.3.15.post5/pygmtsar/ASF.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.3.15.post5/pygmtsar/AWS.py
--rw-r--r--   0 mbg        (501) staff       (20)     7454 2024-03-15 10:56:24.000000 pygmtsar-2024.3.15.post5/pygmtsar/ESA.py
--rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.3.15.post5/pygmtsar/GMT.py
--rw-r--r--   0 mbg        (501) staff       (20)    36536 2024-03-13 06:48:19.000000 pygmtsar-2024.3.15.post5/pygmtsar/IO.py
--rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.3.15.post5/pygmtsar/NCubeVTK.py
--rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.3.15.post5/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.3.15.post5/pygmtsar/PRM_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    18985 2024-03-27 12:16:00.000000 pygmtsar-2024.3.15.post5/pygmtsar/S1.py
--rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack.py
--rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_align.py
--rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_export.py
--rw-r--r--   0 mbg        (501) staff       (20)    18391 2023-11-28 08:51:08.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     6276 2024-03-16 18:59:39.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_multilooking.py
--rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)    46291 2024-03-10 09:58:41.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_phasediff.py
--rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_prm.py
--rw-r--r--   0 mbg        (501) staff       (20)     6255 2024-02-20 05:55:49.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_ps.py
--rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    45060 2024-03-14 11:24:43.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     8884 2024-01-01 15:32:51.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_stl.py
--rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_tidal.py
--rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_topo.py
--rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_trans_inv.py
--rw-r--r--   0 mbg        (501) staff       (20)    26491 2024-03-10 08:58:55.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.3.15.post5/pygmtsar/Stack_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.3.15.post5/pygmtsar/Tiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.3.15.post5/pygmtsar/XYZTiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.3.15.post5/pygmtsar/_Stack_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)     1061 2024-03-27 12:18:22.000000 pygmtsar-2024.3.15.post5/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.3.15.post5/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.3.15.post5/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.3.15.post5/pygmtsar/tqdm_joblib.py
--rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.3.15.post5/pygmtsar/utils.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-03-27 12:19:00.381225 pygmtsar-2024.3.15.post5/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-03-27 12:19:00.000000 pygmtsar-2024.3.15.post5/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     1132 2024-03-27 12:19:00.000000 pygmtsar-2024.3.15.post5/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2024-03-27 12:19:00.000000 pygmtsar-2024.3.15.post5/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      330 2024-03-27 12:19:00.000000 pygmtsar-2024.3.15.post5/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2024-03-27 12:19:00.000000 pygmtsar-2024.3.15.post5/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2024-03-27 12:19:00.381882 pygmtsar-2024.3.15.post5/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-03-08 07:02:25.000000 pygmtsar-2024.3.15.post5/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-06 16:13:18.516048 pygmtsar-2024.3.15.post7/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.3.15.post7/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-06 16:13:18.515703 pygmtsar-2024.3.15.post7/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.3.15.post7/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-06 16:13:18.514343 pygmtsar-2024.3.15.post7/pygmtsar/
+-rw-r--r--   0 mbg        (501) staff       (20)    20813 2024-03-28 13:09:48.000000 pygmtsar-2024.3.15.post7/pygmtsar/ASF.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.3.15.post7/pygmtsar/AWS.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7454 2024-03-15 10:56:24.000000 pygmtsar-2024.3.15.post7/pygmtsar/ESA.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.3.15.post7/pygmtsar/GMT.py
+-rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.3.15.post7/pygmtsar/IO.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.3.15.post7/pygmtsar/NCubeVTK.py
+-rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.3.15.post7/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.3.15.post7/pygmtsar/PRM_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    18986 2024-04-05 07:42:45.000000 pygmtsar-2024.3.15.post7/pygmtsar/S1.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_align.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_export.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_multilooking.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)    47295 2024-03-29 07:29:11.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_phasediff.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_prm.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_ps.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    46250 2024-04-05 20:26:03.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8884 2024-01-01 15:32:51.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_stl.py
+-rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_tidal.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_topo.py
+-rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_trans_inv.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26491 2024-03-10 08:58:55.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.3.15.post7/pygmtsar/Tiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.3.15.post7/pygmtsar/XYZTiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.3.15.post7/pygmtsar/_Stack_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1061 2024-04-05 20:28:55.000000 pygmtsar-2024.3.15.post7/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.3.15.post7/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.3.15.post7/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.3.15.post7/pygmtsar/tqdm_joblib.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.3.15.post7/pygmtsar/utils.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-06 16:13:18.515366 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-06 16:13:18.000000 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     1132 2024-04-06 16:13:18.000000 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-06 16:13:18.000000 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      330 2024-04-06 16:13:18.000000 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-06 16:13:18.000000 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2024-04-06 16:13:18.516100 pygmtsar-2024.3.15.post7/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-03-08 07:02:25.000000 pygmtsar-2024.3.15.post7/setup.py
```

### Comparing `pygmtsar-2024.3.15.post5/LICENSE.txt` & `pygmtsar-2024.3.15.post7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/PKG-INFO` & `pygmtsar-2024.3.15.post7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.3.15.post5
+Version: 2024.3.15.post7
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.3.15.post5/README.md` & `pygmtsar-2024.3.15.post7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,18 @@
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19PLuebOZ4gaYX5ym1H7SwUbJKfl23qPr?usp=sharing) PyGMTSAR Elevation Map:  Erzincan, Türkiye.
 <img src="https://github.com/AlexeyPechnikov/pygmtsar/assets/7342379/066532d5-7b07-49d2-9478-7b8f966a3752" width="100%">
 
 ## PyGMTSAR Live Examples on Google Colab Pro
 
 For subscribers, I share more complex SBAS and PSI use cases on Google Colab Pro through my [Patreon page](https://www.patreon.com/pechnikov). These use cases are suitable for InSAR learners, researchers, and industry specialists working on their challenging projects. Large areas and big stacks for thousands of interferograms, low-coherence territories, and extensive atmospheric phase delays - all these tasks can be addressed with PyGMTSAR. These examples can still be run online on the Google Colab Pro platform, which is cost-effective ($10/month) and provides a good balance between very fast data transfer speeds for downloading dozens of Sentinel-1 SLC scenes, available disk space to store the datasets and process them (approximately 220GB vs. 110GB for the free version of Google Colab), processing speed (8 vCPUs vs. 2 for the free version of Google Colab), and accessible memory (54GB vs. 12GB for the free version of Google Colab). I frequently utilize Google Colab Pro myself to manage up to five parallel InSAR projects, without concerns about disk space, memory, or processing performance limitations. Moreover, all the examples can be executed locally as well as on cloud hosts and remote servers.
 
+## Projects and Publications Using PyGMTSAR
+
+Explore the diverse applications of PyGMTSAR in projects and academic research on the dedicated [Projects and Publications](/pubs/README.md) page.
+
 ## Announcements
 
 **E-Book Release: 'PyGMTSAR: Sentinel-1 Python InSAR: An Introduction'**
 The e-book is now available for the stable PyGMTSAR release across various platforms, including [Amazon, Apple, Kobo, and many other bookstores](https://books2read.com/b/PyGMTSAR-introduction). For a glimpse of the content, check out the [PyGMTSAR Introduction Preview](https://github.com/AlexeyPechnikov/pygmtsar/blob/pygmtsar2/book/PyGMTSAR_preview.pdf) in the GitHub repository.
 
 <img src="https://github.com/AlexeyPechnikov/pygmtsar/assets/7342379/93859fc8-f867-41d0-a03a-0fd89d854e82" width="40%">
```

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/ASF.py` & `pygmtsar-2024.3.15.post7/pygmtsar/ASF.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/AWS.py` & `pygmtsar-2024.3.15.post7/pygmtsar/AWS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/ESA.py` & `pygmtsar-2024.3.15.post7/pygmtsar/ESA.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/GMT.py` & `pygmtsar-2024.3.15.post7/pygmtsar/GMT.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/IO.py` & `pygmtsar-2024.3.15.post7/pygmtsar/IO.py`

 * *Files 0% similar despite different names*

```diff
@@ -707,15 +707,15 @@
         encoding = {varname: self._compression(data[varname].shape[1:]) for varname in data.data_vars}
         #print ('encoding', encoding)
 
         # Applying iterative processing to prevent Dask scheduler deadlocks.
         counter = 0
         digits = len(str(stacksize))
         # Splitting all the pairs into chunks, each containing approximately queue pairs.
-        n_chunks = stacksize // queue if stacksize >= queue else 1
+        n_chunks = stacksize // queue if stacksize > queue else 1
         for chunk in np.array_split(range(stacksize), n_chunks):
             dss = [data.isel({stackvar: ind}) for ind in chunk]
             if stackvar == 'date':
                 stackvals = [ds[stackvar].dt.date.values for ds in dss]
             else:
                 stackvals = [ds[stackvar].item().split(' ') for ds in dss]
             # save to NetCDF file
```

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/NCubeVTK.py` & `pygmtsar-2024.3.15.post7/pygmtsar/NCubeVTK.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/PRM.py` & `pygmtsar-2024.3.15.post7/pygmtsar/PRM.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2024.3.15.post7/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/S1.py` & `pygmtsar-2024.3.15.post7/pygmtsar/S1.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                 else:
                     # in case of data parse or another error
                     raise ValueError(f'Unexpected orbit product {orbit.product}')
     
         # TODO: unzip files
         def download_orbit(basedir, url):
             filename = os.path.join(basedir, os.path.basename(os.path.splitext(url)[0]))
-            print ('url', url, 'filename', filename)
+            #print ('url', url, 'filename', filename)
             with requests.get(url, timeout=S1.http_timeout) as response:
                 response.raise_for_status()
                 with open(filename, 'wb') as f:
                     with zipfile.ZipFile(BytesIO(response.content), 'r') as zip_in:
                         zip_files = zip_in.namelist()
                         if len(zip_files) == 0:
                             raise Exception('ERROR: Downloaded file is empty zip archive.')
```

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_align.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_align.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_base.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_dem.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_detrend.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_detrend.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_export.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_export.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_geocode.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_geocode.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,63 +55,85 @@
     # linear:  coords [array([597.10471665]), array([16977.3737493])]
     # coarsen=4:
     # nearest: coords [array([596.42352295]), array([16978.65625])]
     # linear:  coords [array([597.1080563]), array([16977.35608873])]
     def geocode(self, geometry, z_offset=None):
         """
         Inverse geocode input geodataframe with 2D or 3D points. 
-        
+
         Examples:
         ---------
         sbas.geocode(AOI.assign(col=0))
         sbas.geocode(gpd.GeoDataFrame(geometry=AOI.centroid))
         sbas.geocode(AOI.centroid)
         sbas.geocode(AOI.geometry.item())
         sbas.geocode([AOI.geometry.item()])
         sbas.geocode(geometry)
+        
+        sbas.geocode(AOI).plot()
+        sbas.geocode(AOI.boundary.buffer(0.0001)).plot(color='g', alpha=0.5, ax=plt.gca())
+        sbas.geocode(AOI.boundary).plot(color='r', ax=plt.gca())
+        sbas.geocode(POI).plot(color='r', ax=plt.gca())
         """
         import numpy as np
         import geopandas as gpd
         import xarray as xr
-        from shapely.geometry import LineString, Point
-
+        from shapely.geometry import Point, LineString, Polygon
+    
         if isinstance(geometry, (gpd.GeoDataFrame, gpd.GeoSeries)):
             geometries = geometry.geometry
         elif isinstance(geometry, (list, tuple, np.ndarray)):
             geometries = geometry
         else:
             geometries = [geometry]
-
+    
         dem = self.get_dem()
         prm = self.PRM()
     
-        geoms = []
-        for geom in geometries:
-            #print (geom)
-            coords = np.asarray(geom.coords[:])
+        def coords_transform(coords):
+            # uses external variables dem, prm
             #print (len(coords))
             ele = dem.interp(lat=xr.DataArray(coords[:,1]),
                        lon=xr.DataArray(coords[:,0]), method='linear').compute()
             if z_offset is None:
                 z = coords[:,2] if coords.shape[1]==3 else 0
             else:
                 z = z_offset
-            points_ll = np.column_stack([coords[:,0], coords[:,1], ele.values + z])
-            #print (points_ll)
-            points_ra = prm.SAT_llt2rat(points_ll)
-            points_ra = points_ra[:,:2] if len(points_ll)>1 else [points_ra[:2]]
-            #print (points_ra)
+            coords_ll = np.column_stack([coords[:,0], coords[:,1], ele.values + z])
+            #print (coords_ll)
+            coords_ra = prm.SAT_llt2rat(coords_ll)
+            coords_ra = coords_ra[:,:2] if len(coords_ll)>1 else [coords_ra[:2]]
+            #print (coords_ra)
+            return coords_ra
+    
+        geoms = []
+        for geom in geometries:
+            #print (geom)
             geom_type = geom.type
             if geom_type == 'LineString':
-                geom = LineString(points_ra)
+                coords = np.asarray(geom.coords[:])
+                geom = LineString(coords_transform(coords))
             elif geom_type == 'Point':
-                geom = Point(points_ra)
+                coords = np.asarray(geom.coords[:])
+                geom = Point(coords_transform(coords))
+            elif geom_type == 'Polygon':
+                exterior_coords = np.asarray(geom.exterior.coords)
+                interiors_coords = [np.asarray(interior.coords) for interior in geom.interiors]
+                geom = Polygon(coords_transform(exterior_coords), [coords_transform(icoords) for icoords in interiors_coords])
+    #         elif geom_type == 'MultiPolygon':
+    #             polygons = []
+    #             for part in geom:
+    #                 ...
+    #                 polygons.append(Polygon(exterior, interiors))
+    #             geom = MultiPolygon(polygons)
+            else:
+                raise Exception(f'ERROR:: unsupported geometry type {geom_type}. Expected Point, LineString, Polygon.')
             #print (geom)
             geoms.append(geom)
-
+    
         # preserve original dataframe columns if exists
         if isinstance(geometry, gpd.GeoDataFrame):
             return gpd.GeoDataFrame(geometry, geometry=geoms, crs=3857)
         elif isinstance(geometry, gpd.GeoSeries):
             return gpd.GeoSeries(geoms, crs=3857)
         elif isinstance(geometry, (list, tuple, np.ndarray)):
             return geoms
```

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_incidence.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_landmask.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_landmask.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             os.remove(landmask_filename)
         encoding = {'landmask': self._compression(landmask.shape)}
         landmask.rename('landmask').load()\
             .to_netcdf(landmask_filename, encoding=encoding, engine=self.netcdf_engine)
 
         self.landmask_filename = landmask_filename
 
-    def plot_landmask(self, landmask='auto', caption='Land Mask', cmap='binary', aspect=None, **kwargs):
+    def plot_landmask(self, landmask='auto', caption='Land Mask', cmap='binary_r', aspect=None, **kwargs):
         import matplotlib.pyplot as plt
 
         if isinstance(landmask, str) and landmask == 'auto':
             landmask = self.get_landmask()
 
         plt.figure()
         landmask.plot.imshow(vmin=0, cmap=cmap)
```

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_multilooking.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_multilooking.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_orbits.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_phasediff.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_phasediff.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,56 +10,65 @@
 from .Stack_topo import Stack_topo
 from .tqdm_dask import tqdm_dask
 from .PRM import PRM
 
 class Stack_phasediff(Stack_topo):
 
     def compute_interferogram(self, pairs, name, resolution=None, weight=None, phase=None, wavelength=None,
-                              psize=None, coarsen=None, queue=None, timeout=None, debug=False):
+                              psize=None, coarsen=None, queue=None, timeout=None,
+                              skip_exist=False, joblib_backend=None, debug=False):
         import xarray as xr
         import numpy as np
         import dask
         # cleanup unused resources before start
         import gc; gc.collect()
-
-        # delete stack files if exist
-        self.delete_stack(name)
-
+    
+        if not skip_exist:
+            # delete stack files if exist
+            self.delete_stack(name)
+    
         # define anti-aliasing filter for the specified output resolution
         if wavelength is None:
             wavelength = resolution
-
+    
         if queue is None:
             queue = self.netcdf_queue
         if queue is None:
             # process all the pairs in a single operation
             queue = len(pairs)
-
+    
         # decimate the 1:4 multilooking grids to specified resolution
         if resolution is not None:
             decimator = self.decimator(resolution=resolution, grid=coarsen, debug=debug)
         else:
             decimator = None
     
         # Applying iterative processing to prevent Dask scheduler deadlocks.
         counter = 0
         digits = len(str(len(pairs)))
         # Splitting all the pairs into chunks, each containing approximately queue pairs.
-        n_chunks = len(pairs) // queue if len(pairs) >= queue else 1
-        for chunk in np.array_split(pairs, n_chunks):
+        #n_chunks = len(pairs) // queue if len(pairs) >= queue else 1
+        if len(pairs) > queue:
+            chunks = [pairs[i:i + queue] for i in range(0, len(pairs), queue)]
+            n_chunks = len(chunks)
+        else:
+            chunks = [pairs]
+            n_chunks = 1
+        #for chunk in np.array_split(pairs, n_chunks):
+        for chunk in chunks:
             #print (f'Interferogram pairs: {len(pairs)}')
             chunk, dates = self.get_pairs(chunk, dates=True)
             # load Sentinel-1 data
             data = self.open_data(dates, debug=debug)
             intensity = np.square(np.abs(data))
             # Gaussian filtering 200m cut-off wavelength with optional range multilooking on Sentinel-1 amplitudes
             amp_look = self.multilooking(intensity, wavelength=wavelength, coarsen=coarsen, debug=debug)
             del intensity
             # calculate phase difference with topography correction
-            phasediff = self.phasediff(chunk, data, phase=phase, debug=debug)
+            phasediff = self.phasediff(chunk, data, phase=phase, joblib_backend=joblib_backend, debug=debug)
             del data
             # Gaussian filtering 200m cut-off wavelength with optional range multilooking
             phasediff_look = self.multilooking(phasediff, weight=weight,
                                                wavelength=wavelength, coarsen=coarsen, debug=debug)
             del phasediff
             # correlation with optional range decimation
             corr_look = self.correlation(phasediff_look, amp_look, debug=debug)
@@ -84,32 +93,36 @@
                 intf_dec = decimator(intf_look)
                 corr_dec = decimator(corr_look)
                 out = xr.merge([intf_dec, corr_dec])
                 del intf_dec, corr_dec
             else:
                 out = xr.merge([intf_look, corr_look])
             del corr_look, intf_look
-            self.save_stack(out, name, timeout=timeout,
-                            caption=f'Saving Interferogram {(counter+1):0{digits}}...{(counter+len(chunk)):0{digits}} from {len(pairs)}')
+            caption = f'Saving Interferogram {(counter+1):0{digits}}...{(counter+len(chunk)):0{digits}} from {len(pairs)}'
+            self.save_stack(out, name, caption=caption, queue=queue, timeout=timeout)
             counter += len(chunk)
             del out, chunk, dates
 
     # single-look interferogram processing has a limited set of arguments
     # resolution and coarsen are not applicable here
     def compute_interferogram_singlelook(self, pairs, name, weight=None, phase=None, wavelength=None, psize=None,
-                                         queue=16, timeout=None, debug=False):
+                                         queue=16, timeout=None,
+                                         skip_exist=False, joblib_backend=None, debug=False):
         self.compute_interferogram(pairs, name, weight=weight, phase=phase, wavelength=wavelength,
-                                   psize=psize, queue=queue, timeout=timeout, debug=debug)
+                                   psize=psize, queue=queue, timeout=timeout,
+                                   skip_exist=skip_exist, joblib_backend=joblib_backend, debug=debug)
 
     # Goldstein filter requires square grid cells means 1:4 range multilooking.
     # For multilooking interferogram we can use square grid always using coarsen = (1,4)
-    def compute_interferogram_multilook(self, pairs, name, resolution=None, weight=None, phase=None,
-                                        wavelength=None, psize=None, coarsen=(1,4), queue=16, timeout=None, debug=False):
+    def compute_interferogram_multilook(self, pairs, name, resolution=None, weight=None, phase=None, wavelength=None,
+                                        psize=None, coarsen=(1,4), queue=16, timeout=None,
+                                        skip_exist=False, joblib_backend=None, debug=False):
         self.compute_interferogram(pairs, name, resolution=resolution, weight=weight, phase=phase, wavelength=wavelength,
-                                   psize=psize, coarsen=coarsen, queue=queue, timeout=timeout, debug=debug)
+                                   psize=psize, coarsen=coarsen, queue=queue, timeout=timeout,
+                                   skip_exist=skip_exist, joblib_backend=joblib_backend, debug=debug)
 
     @staticmethod
     def interferogram(phase, debug=False):
         import numpy as np
 
         if debug:
             print ('DEBUG: interferogram')
@@ -412,30 +425,35 @@
 # 
 #         coord_pair = [' '.join(pair) for pair in pairs]
 #         coord_ref = xr.DataArray(pd.to_datetime(pairs[:,0]), coords={'pair': coord_pair})
 #         coord_rep = xr.DataArray(pd.to_datetime(pairs[:,1]), coords={'pair': coord_pair})
 # 
 #         return xr.concat(stack, dim='pair').assign_coords(ref=coord_ref, rep=coord_rep, pair=coord_pair).rename('phasediff')
 
-    def phasediff(self, pairs, data='auto', topo='auto', phase=None, method='nearest', debug=False):
+    def phasediff(self, pairs, data='auto', topo='auto', phase=None, method='nearest', joblib_backend=None, debug=False):
         import pandas as pd
         import dask
         import dask.dataframe
         import xarray as xr
         import numpy as np
         #from tqdm.auto import tqdm
         import joblib
+        from joblib.externals import loky
+        loky.get_reusable_executor(kill_workers=True).shutdown(wait=True)
         import warnings
         # suppress Dask warning "RuntimeWarning: invalid value encountered in divide"
         warnings.filterwarnings('ignore')
         warnings.filterwarnings('ignore', module='dask')
         warnings.filterwarnings('ignore', module='dask.core')
 
         if debug:
             print ('DEBUG: phasediff')
+        
+        if joblib_backend is None and debug:
+            joblib_backend = 'sequential'
 
         # convert pairs (list, array, dataframe) to 2D numpy array
         pairs, dates = self.get_pairs(pairs, dates=True)
         pairs = pairs[['ref', 'rep']].astype(str).values
 
         if isinstance(topo, str) and topo == 'auto':
             topo = self.get_topo()
@@ -637,15 +655,15 @@
             prm1 = self.PRM(date1)
             prm2 = self.PRM(date2)
             prm2.set(prm1.SAT_baseline(prm2, tail=9)).fix_aligned()
             prm1.set(prm1.SAT_baseline(prm1).sel('SC_height','SC_height_start','SC_height_end')).fix_aligned()
             return {(date1, date2): (prm1, prm2)}
 
         #with self.tqdm_joblib(tqdm(desc=f'Pre-Processing PRM', total=len(pairs))) as progress_bar:
-        prms = joblib.Parallel(n_jobs=-1)(joblib.delayed(prepare_prms)(pair) for pair in pairs)
+        prms = joblib.Parallel(n_jobs=-1, backend=joblib_backend)(joblib.delayed(prepare_prms)(pair) for pair in pairs)
         # convert the list of dicts to a single dict
         prms = {k: v for d in prms for k, v in d.items()}
 
         if isinstance(data, str) and data == 'auto':
             # open datafiles required for all the pairs
             data = self.open_data(dates)
```

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_prm.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_prm.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_ps.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_ps.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
 from .Stack_stl import Stack_stl
 from .tqdm_dask import tqdm_dask
 
 class Stack_ps(Stack_stl):
 
-    def get_ps(self):
-        return self.open_cube('ps')
+    def get_ps(self, name='ps'):
+        return self.open_cube(name)
 
     #from pygmtsar import tqdm_dask
     #Stack.ps = ps    
     #stack.ps(interactive=True)
     #stack.ps()
     #adi = stack.open_grids(None, 'ps')
     #adi
     #ps_decimator = stack.pixel_decimator(resolution=60, grid=adi, debug=True)
     #adi_dec = adi.coarsen({'y': 4, 'x': 16}, boundary='trim').min()
     #adi_dec
     # define PS candidates using Amplitude Dispersion Index (ADI)
-    def compute_ps(self, dates=None, data='auto'):
+    def compute_ps(self, dates=None, data='auto', name='ps', interactive=False):
         import xarray as xr
         import numpy as np
         import dask
         import os
         import warnings
         # suppress Dask warning "RuntimeWarning: invalid value encountered in divide"
         warnings.filterwarnings('ignore')
@@ -45,25 +45,27 @@
         # dask.persist returns tuple
         norm = mean[0].mean(dim='date') / mean[0]
         # compute average and std.dev.
         stats = (norm * data).pipe(lambda x: (x.mean(dim='date'), x.std(dim='date')))
         del data, norm
         ds = xr.merge([stats[0].rename('average'), stats[1].rename('deviation'), mean[0].rename('stack_average')])
         del stats, mean
-        self.save_cube(ds, 'ps', 'Compute Stability Measures')
+        if interactive:
+            return ds
+        self.save_cube(ds, name, 'Compute Stability Measures')
         del ds
 
-    def psfunction(self, ps='auto'):
+    def psfunction(self, ps='auto', name='ps'):
         import numpy as np
         if isinstance(ps, str) and ps == 'auto':
-            ps = self.get_ps()
+            ps = self.get_ps(name)
         psfunction = (ps.average/(2*ps.deviation))
         return psfunction.where(np.isfinite(psfunction)).rename('psf')
 
-    def plot_psfunction(self, psfunction='auto', cmap='gray', quantile=None, vmin=None, vmax=None, **kwargs):
+    def plot_psfunction(self, psfunction='auto', caption='PS Function', cmap='gray', quantile=None, vmin=None, vmax=None, **kwargs):
         import numpy as np
         import matplotlib.pyplot as plt
 
         if isinstance(psfunction, str) and psfunction == 'auto':
             psfunction = self.psfunction()
 
         if quantile is not None:
@@ -72,15 +74,15 @@
         if quantile is not None:
             vmin, vmax = np.nanquantile(psfunction, quantile)
 
         plt.figure()
         psfunction.plot.imshow(cmap=cmap, vmin=vmin, vmax=vmax)
         self.plot_AOI(**kwargs)
         self.plot_POI(**kwargs)
-        plt.title('PS Function')
+        plt.title(caption)
 
 #     def get_adi_threshold(self, threshold):
 #         """
 #         Vectorize Amplitude Dispersion Index (ADI) raster values selected using the specified threshold.
 #         """
 #         import numpy as np
 #         import dask
```

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_reframe.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_reframe_gmtsar.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_sbas.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_sbas.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,85 +331,86 @@
                 df = df[(df['ref'].isin(dates))&(df['rep'].isin(dates))]
 
         if limit[1] is not None:
             print ('TODO: process upper limit')
 
         return df
 
-    def sbas_pairs(self, days=100, meters=None, invert=False):
+    def sbas_pairs(self, days=100, meters=None, invert=False, dates=None):
         """
         Generates a sorted list of baseline pairs based on specified temporal and spatial criteria.
-
+    
         This function creates a list of baseline pairs for Sentinel-1 data, considering the given
         temporal and spatial constraints. The list includes pairs that meet the specified days and
         meters criteria.
-
+    
         Parameters
         ----------
         days : int, optional
             Maximum temporal separation between image pairs in days (default is 100).
         meters : int, optional
             Maximum spatial separation between image pairs in meters (default is None).
         invert : bool, optional
             If True, invert the order of reference and repeat images (default is False).
-
+    
         Returns
         -------
         pandas.DataFrame
             A DataFrame containing the sorted list of baseline pairs with reference and repeat dates,
             timelines, and baselines.
-
+    
         """
         import numpy as np
         import pandas as pd
-
-        def baseline_table():
+    
+        def baseline_table(dates):
             """
             Generates a baseline table for Sentinel-1 data, containing dates, times, and baseline components.
-
+    
             This function creates a baseline table for Sentinel-1 data by processing the PRM files, which
             contain metadata for each image. The table includes dates, times, and parallel and perpendicular
             baseline components for each image.
             """
             import pandas as pd
             import numpy as np
-
-            datetimes = self.df.datetime
-
+    
             prm_ref = self.PRM()
             data = []
-            for (date, dt) in datetimes.items():
+            for date in dates:
                 prm_rep = self.PRM(date)
                 BPL, BPR = prm_ref.SAT_baseline(prm_rep).get('B_parallel', 'B_perpendicular')
                 data.append({'date':date, 'BPL':BPL, 'BPR':BPR})
             df = pd.DataFrame(data).set_index('date')
             df.index = pd.DatetimeIndex(df.index)
             return df
-
-        tbl = baseline_table()
+    
+        if dates is None:
+            dates = self.df.index
+    
+        tbl = baseline_table(dates)
         data = []
         for line1 in tbl.itertuples():
             counter = 0
             for line2 in tbl.itertuples():
                 #print (line1, line2)
                 if not (line1.Index < line2.Index and (line2.Index - line1.Index).days < days + 1):
                     continue
                 if meters is not None and not (abs(line1.BPR - line2.BPR)< meters + 1):
                     continue
-
+    
                 counter += 1
                 if not invert:
                     data.append({'ref':line1.Index, 'rep': line2.Index,
                                  'ref_baseline': np.round(line1.BPR, 2),
                                  'rep_baseline': np.round(line2.BPR, 2)})
                 else:
                     data.append({'ref':line2.Index, 'rep': line1.Index,
                                  'ref_baseline': np.round(line2.BPR, 2),
                                  'rep_baseline': np.round(line1.BPR, 2)})
-
+    
         df = pd.DataFrame(data).sort_values(['ref', 'rep'])
         return df.assign(pair=[f'{ref} {rep}' for ref, rep in zip(df['ref'].dt.date, df['rep'].dt.date)],
                          baseline=df.rep_baseline - df.ref_baseline,
                          duration=(df['rep'] - df['ref']).dt.days,
                          rel=np.datetime64('nat'))
 
     def sbas_pairs_extend(self, baseline_pairs):
@@ -744,66 +745,74 @@
 
     def plot_baseline_deviation(self, baseline_pairs, pairs_best=None, column='stddev'):
         #print ('NOTE: this function is deprecated, use instead Stack.plot_baseline_attribute()')
         self.plot_baseline_attribute(baseline_pairs, pairs_best, column=column, caption='Baseline Deviation')
 
     def plot_baseline_displacement(self, phase, corr=None, caption=None, cmap='turbo',
                                    displacement=True, unwrap=True,
-                                   stl=False, stl_freq='W', stl_periods=52, stl_robust=True, tolerance=np.pi/2):
+                                   stl=False, stl_freq='W', stl_periods=52, stl_robust=True,
+                                   los=False, tolerance=np.pi/2, xlabel_rotation=45):
         """
         Performs 1D unwrapping, linear regression, and STL on a given set of phase values.
-
+    
         The linear regression model is represented as:
             y = β0 + β1 * x
-
+    
         Where:
             y: Dependent variable (the outcome being predicted).
             x: Independent variable (the predictor).
             β0: Intercept (the value of y when x is 0).
             β1: Slope or "velocity" (the rate of change in y for a one-unit change in x).
-
+    
         In this model, 'β' (beta) symbols followed by indices (0, 1, 2, ...) represent 
         the coefficients in the regression equation. β0 is always the intercept, and 
         β1, β2, etc., represent the coefficients of the predictor variables.
-
+    
         """
         import numpy as np
         import xarray as xr
         import pandas as pd
         from scipy.stats import linregress
         import matplotlib
         import matplotlib.pyplot as plt
         from matplotlib.cm import ScalarMappable
-
+    
         if not displacement and stl:
             print ("NOTE: Displacement is automatically set to 'True' because it is required for 'stl=True'.")
         assert isinstance(phase, xr.DataArray) and phase.dims == ('pair',), \
             'ERROR: Argument phase should be 1D Xarray with "pair" dimension'
         plt.figure()
         colors = matplotlib.cm.get_cmap(cmap)
-
+    
         df = phase.to_dataframe()
         df['corr'] = corr.values if corr is not None else 1
         pairs, dates = self.get_pairs(phase, dates=True)
         dates = pd.DatetimeIndex(dates)
         matrix = self.lstsq_matrix(pairs)
-
+    
         if unwrap:
             df['phase'] = self.unwrap_pairs(phase.values, df['corr'].values, matrix, tolerance)
-
+        
+        unit = 'rad'
+        name = 'Phase'
+        if los:
+            df['phase'] = self.los_displacement_mm(df['phase'])
+            unit = 'mm'
+            name = 'Displacement'
+    
         if displacement or stl:
             solution = self.lstsq1d(df['phase'].values, 0.999*df['corr'].values if corr is not None else None, matrix)
             #print ('solution', solution)
             days = (dates - dates[0]).days
             #print ('days', days)
             slope, intercept, r_value, p_value, std_err = linregress(days, solution)
             #print (slope, intercept, r_value, p_value, std_err)
             velocity = np.round(slope*365.25, 2)
             values = intercept + slope*days
-
+    
         if stl:
             #assert displacement, 'ERROR: Argument value stl=True requires argument displacement=True'
             dt, dt_periodic = self.stl_periodic(dates, stl_freq)
             trend, seasonal, resid = self.stl1d(solution, dt, dt_periodic, periods=stl_periods, robust=stl_robust)
             #years = ((dt_periodic.date[-1] - dt_periodic.date[0]).dt.days/365.25).item()
             stl_dates = pd.to_datetime(dt_periodic)
             stl_days = (stl_dates - stl_dates[0]).days
@@ -811,15 +820,15 @@
             stl_slope, stl_intercept, stl_r_value, stl_p_value, stl_std_err = linregress(stl_days, trend)
             #print (stl_slope, stl_intercept, stl_r_value, stl_p_value, stl_std_err)
             stl_velocity = np.round(stl_slope*365.25, 2)
             # for linear trend
             #velocity = (trend[-1] - trend[0])/years
             # for integral trend
             #velocity = np.round(years*np.nansum(trend - np.nanmin(trend))/trend.size, 2)
-
+    
         vmin = df['phase'].min()
         vmax = df['phase'].max()
         y_min = y_max = 0
         dts = []
         idx = -1
         errors = []
         for i, row in df.iterrows():
@@ -855,43 +864,54 @@
             #print ('weights', weights)
             #print (errors.size, weights.size, errors)
             #rmse = np.sqrt(np.sum(errors**2) / errors.size)
             rmse = np.sqrt(np.sum(weights * (errors**2)) / np.sum(weights) / errors.size)
             #print ('weighted PI-scaled rmse', np.round(rmse / np.pi, 2))
             plt.plot(dates, solution, color='black', linestyle='--', linewidth=2, label='LSQ')
             plt.plot(dates, values, color='blue', linestyle='-', linewidth=2,
-                     label=f'LSQ β1 {velocity:0.1f} and β0={intercept:0.1f} [rad/year], P-value={p_value:0.2f}')
-
+                     label=f'LSQ β1 {velocity:0.1f} and β0={intercept:0.1f} [{unit}/year], P-value={p_value:0.2f}')
+    
         if stl:
             plt.plot(dt_periodic.date, trend, color='blue', linestyle='--', linewidth=2,
-                     label=f'STL β1 {stl_velocity:0.1f} and β0={stl_intercept:0.1f} [rad/year]')
+                     label=f'STL β1 {stl_velocity:0.1f} and β0={stl_intercept:0.1f} [{unit}/year]')
             plt.plot(dt_periodic.date, seasonal, color='green', linestyle='--', linewidth=1, label='STL Seasonal')
             plt.plot(dt_periodic.date, resid, color='red', linestyle='--', linewidth=1, label='STL Residual')
-
+    
         plt.grid(axis='y')
-        y_min = np.floor(y_min / np.pi) * np.pi
-        y_max = np.ceil(y_max / np.pi) * np.pi
-        y_ticks = np.arange(y_min, y_max + np.pi, np.pi)
-        plt.yticks(y_ticks, [f'{y:.0f}π' if y != 0 else '0' for y in y_ticks / np.pi])
-
+        if unit == 'rad':
+            y_min = np.floor(y_min / np.pi) * np.pi
+            y_max = np.ceil(y_max / np.pi) * np.pi
+            y_ticks = np.arange(y_min, y_max + np.pi, np.pi)
+            plt.yticks(y_ticks, [f'{y:.0f}π' if y != 0 else '0' for y in y_ticks / np.pi])
+    
         if corr is not None:
             sm = ScalarMappable(cmap=colors, norm=plt.Normalize(vmin=0, vmax=1))
             sm.set_array([])
             cbar = plt.colorbar(sm, ax=plt.gca(), orientation='vertical')
             cbar.set_label('Correlation')
-
+    
+        plt.xticks(rotation=xlabel_rotation)
         plt.xlabel('Timeline')
-        plt.ylabel('Phase, [rad]')
+        plt.ylabel(f'{name}, [{unit}]')
         plt.title('Displacement' \
-                  + (f' RMSE={rmse:0.3f} [rad]' if displacement or stl else '') \
+                  + (f' RMSE={rmse:0.3f} [{unit}]' if displacement or stl else '') \
                   + (f'\n{caption}' if caption is not None else ''))
         plt.xlim([dates[0], dates[-1]])
         if displacement or stl:
             plt.legend()
 
+    def plot_baseline_displacement_los_mm(self, phase, corr=None, caption=None, cmap='turbo',
+                                   displacement=True, unwrap=True,
+                                   stl=False, stl_freq='W', stl_periods=52, stl_robust=True,
+                                   tolerance=np.pi/2, xlabel_rotation=45):
+        self.plot_baseline_displacement(phase=phase, corr=corr, caption=caption, cmap=cmap,
+                                   displacement=displacement, unwrap=unwrap,
+                                   stl=stl, stl_freq=stl_freq, stl_periods=stl_periods, stl_robust=stl_robust,
+                                   los=True, tolerance=tolerance, xlabel_rotation=xlabel_rotation)
+
     def rmse(self, data, solution, weight=None):
         """
         Calculate difference between pairs and dates
     
         Use to calculate solution vs pair unwrapped phases difference as
         diff = sbas.stack_vs_cube(phase_unwrap, solution)
         error = np.sqrt(sbas.wrap(diff)**2).sum('pair')
```

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_stl.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_stl.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_tidal.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_tidal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_topo.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_topo.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_trans.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_trans_inv.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_trans_inv.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_unwrap.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_unwrap.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Stack_unwrap_snaphu.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Stack_unwrap_snaphu.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/Tiles.py` & `pygmtsar-2024.3.15.post7/pygmtsar/Tiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/XYZTiles.py` & `pygmtsar-2024.3.15.post7/pygmtsar/XYZTiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/_Stack_merge.py` & `pygmtsar-2024.3.15.post7/pygmtsar/_Stack_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/__init__.py` & `pygmtsar-2024.3.15.post7/pygmtsar/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 
 # This file is part of the PyGMTSAR project: https://github.com/mobigroup/gmtsar
 # 
 # Copyright (c) 2023, Alexey Pechnikov
 # 
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
-__version__ = '2024.3.15.post5'
+__version__ = '2024.3.15.post7'
 
 # unified progress indicators
 from .tqdm_joblib import tqdm_joblib
 from .tqdm_dask import tqdm_dask
 # base NetCDF operations and parameters on NetCDF grid
 from .datagrid import datagrid
 # top level module classes
```

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/datagrid.py` & `pygmtsar-2024.3.15.post7/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/tqdm_dask.py` & `pygmtsar-2024.3.15.post7/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/tqdm_joblib.py` & `pygmtsar-2024.3.15.post7/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar/utils.py` & `pygmtsar-2024.3.15.post7/pygmtsar/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2024.3.15.post7/pygmtsar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.3.15.post5
+Version: 2024.3.15.post7
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.3.15.post5/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2024.3.15.post7/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post5/setup.py` & `pygmtsar-2024.3.15.post7/setup.py`

 * *Files identical despite different names*

