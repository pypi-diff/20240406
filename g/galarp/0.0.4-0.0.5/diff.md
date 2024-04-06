# Comparing `tmp/galarp-0.0.4.tar.gz` & `tmp/galarp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galarp-0.0.4.tar", last modified: Wed Apr  3 20:45:50 2024, max compression
+gzip compressed data, was "galarp-0.0.5.tar", last modified: Sat Apr  6 17:11:23 2024, max compression
```

## Comparing `galarp-0.0.4.tar` & `galarp-0.0.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-03 20:45:50.359531 galarp-0.0.4/
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1086 2024-03-26 19:05:50.000000 galarp-0.0.4/LICENSE
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1421 2024-04-03 20:45:50.359248 galarp-0.0.4/PKG-INFO
--rw-r--r--   0 hsouchereau   (503) staff       (20)      611 2024-04-01 22:50:27.000000 galarp-0.0.4/README.rst
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-03 20:45:50.353632 galarp-0.0.4/galarp/
--rw-r--r--   0 hsouchereau   (503) staff       (20)      534 2024-04-03 20:45:27.000000 galarp-0.0.4/galarp/__init__.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-03 20:45:50.355340 galarp-0.0.4/galarp/builtins/
--rw-r--r--   0 hsouchereau   (503) staff       (20)       99 2024-04-02 14:39:40.000000 galarp-0.0.4/galarp/builtins/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     2182 2024-04-02 20:57:13.000000 galarp-0.0.4/galarp/builtins/events.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1342 2024-03-28 20:47:49.000000 galarp-0.0.4/galarp/builtins/hosts.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      691 2024-03-28 18:25:11.000000 galarp-0.0.4/galarp/builtins/initconditions.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1118 2024-04-01 17:27:27.000000 galarp-0.0.4/galarp/builtins/satellites.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-03 20:45:50.355799 galarp-0.0.4/galarp/builtins/tests/
--rw-r--r--   0 hsouchereau   (503) staff       (20)        1 2024-03-28 13:54:47.000000 galarp-0.0.4/galarp/builtins/tests/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1373 2024-04-02 14:10:30.000000 galarp-0.0.4/galarp/builtins/tests/test_builtins.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      473 2024-04-02 14:33:42.000000 galarp-0.0.4/galarp/builtins/tests/test_events.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1396 2024-04-03 16:46:44.000000 galarp-0.0.4/galarp/densities.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-03 20:45:50.356801 galarp-0.0.4/galarp/hosts/
--rw-r--r--   0 hsouchereau   (503) staff       (20)       80 2024-03-29 15:07:15.000000 galarp-0.0.4/galarp/hosts/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      880 2024-03-29 16:44:51.000000 galarp-0.0.4/galarp/hosts/densities.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     3200 2024-04-02 20:57:13.000000 galarp-0.0.4/galarp/hosts/hostorbits.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      264 2024-04-01 15:16:44.000000 galarp-0.0.4/galarp/hosts/initconditions.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     9502 2024-04-02 15:26:47.000000 galarp-0.0.4/galarp/particle_grids.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-03 20:45:50.357101 galarp-0.0.4/galarp/postprocessing/
--rw-r--r--   0 hsouchereau   (503) staff       (20)       70 2024-04-01 22:01:07.000000 galarp-0.0.4/galarp/postprocessing/__init__.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-03 20:45:50.357721 galarp-0.0.4/galarp/postprocessing/plotting/
--rw-r--r--   0 hsouchereau   (503) staff       (20)      206 2024-04-03 14:34:47.000000 galarp-0.0.4/galarp/postprocessing/plotting/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     6382 2024-04-01 22:20:36.000000 galarp-0.0.4/galarp/postprocessing/plotting/general_plots.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     4212 2024-04-03 14:45:50.000000 galarp-0.0.4/galarp/postprocessing/plotting/matrix_plots.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-03 20:45:50.358000 galarp-0.0.4/galarp/postprocessing/plotting/tests/
--rw-r--r--   0 hsouchereau   (503) staff       (20)        0 2024-04-02 14:01:03.000000 galarp-0.0.4/galarp/postprocessing/plotting/tests/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      656 2024-04-02 15:27:47.000000 galarp-0.0.4/galarp/postprocessing/plotting/tests/test_genplots.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1753 2024-04-02 15:28:05.000000 galarp-0.0.4/galarp/postprocessing/plotting/utils.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     4734 2024-04-01 21:48:21.000000 galarp-0.0.4/galarp/postprocessing/utils.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     6420 2024-04-03 16:44:36.000000 galarp-0.0.4/galarp/rampressure.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     8030 2024-03-26 19:05:50.000000 galarp-0.0.4/galarp/shadows.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-03 20:45:50.358905 galarp-0.0.4/galarp/tests/
--rw-r--r--   0 hsouchereau   (503) staff       (20)        0 2024-03-26 19:05:50.000000 galarp-0.0.4/galarp/tests/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      693 2024-04-01 16:19:47.000000 galarp-0.0.4/galarp/tests/helpers.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      747 2024-04-02 15:42:16.000000 galarp-0.0.4/galarp/tests/test_grids.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      519 2024-04-02 15:29:05.000000 galarp-0.0.4/galarp/tests/test_shadows.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1201 2024-04-02 15:31:07.000000 galarp-0.0.4/galarp/tests/test_utils.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      732 2024-04-02 20:57:13.000000 galarp-0.0.4/galarp/tests/test_winds.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      659 2024-03-28 21:18:39.000000 galarp-0.0.4/galarp/tests.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     3435 2024-04-01 22:30:08.000000 galarp-0.0.4/galarp/utils.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     5364 2024-04-03 15:25:22.000000 galarp-0.0.4/galarp/winds.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-03 20:45:50.354569 galarp-0.0.4/galarp.egg-info/
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1421 2024-04-03 20:45:50.000000 galarp-0.0.4/galarp.egg-info/PKG-INFO
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1210 2024-04-03 20:45:50.000000 galarp-0.0.4/galarp.egg-info/SOURCES.txt
--rw-r--r--   0 hsouchereau   (503) staff       (20)        1 2024-04-03 20:45:50.000000 galarp-0.0.4/galarp.egg-info/dependency_links.txt
--rw-r--r--   0 hsouchereau   (503) staff       (20)       30 2024-04-03 20:45:50.000000 galarp-0.0.4/galarp.egg-info/requires.txt
--rw-r--r--   0 hsouchereau   (503) staff       (20)        7 2024-04-03 20:45:50.000000 galarp-0.0.4/galarp.egg-info/top_level.txt
--rw-r--r--   0 hsouchereau   (503) staff       (20)      139 2024-03-28 20:47:19.000000 galarp-0.0.4/pyproject.toml
--rw-r--r--   0 hsouchereau   (503) staff       (20)       38 2024-04-03 20:45:50.359585 galarp-0.0.4/setup.cfg
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1207 2024-03-28 20:28:33.000000 galarp-0.0.4/setup.py
+drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-06 17:11:23.541757 galarp-0.0.5/
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     1086 2024-03-26 19:05:50.000000 galarp-0.0.5/LICENSE
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     1534 2024-04-06 17:11:23.541525 galarp-0.0.5/PKG-INFO
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      611 2024-04-01 22:50:27.000000 galarp-0.0.5/README.rst
+drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-06 17:11:23.536601 galarp-0.0.5/galarp/
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      534 2024-04-06 17:11:18.000000 galarp-0.0.5/galarp/__init__.py
+drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-06 17:11:23.538182 galarp-0.0.5/galarp/builtins/
+-rw-r--r--   0 hsouchereau   (503) staff       (20)       99 2024-04-02 14:39:40.000000 galarp-0.0.5/galarp/builtins/__init__.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     2182 2024-04-02 20:57:13.000000 galarp-0.0.5/galarp/builtins/events.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     1342 2024-03-28 20:47:49.000000 galarp-0.0.5/galarp/builtins/hosts.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      691 2024-03-28 18:25:11.000000 galarp-0.0.5/galarp/builtins/initconditions.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     1118 2024-04-01 17:27:27.000000 galarp-0.0.5/galarp/builtins/satellites.py
+drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-06 17:11:23.538630 galarp-0.0.5/galarp/builtins/tests/
+-rw-r--r--   0 hsouchereau   (503) staff       (20)        1 2024-03-28 13:54:47.000000 galarp-0.0.5/galarp/builtins/tests/__init__.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     1373 2024-04-02 14:10:30.000000 galarp-0.0.5/galarp/builtins/tests/test_builtins.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      473 2024-04-02 14:33:42.000000 galarp-0.0.5/galarp/builtins/tests/test_events.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     2635 2024-04-06 16:51:26.000000 galarp-0.0.5/galarp/densities.py
+drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-06 17:11:23.539214 galarp-0.0.5/galarp/hosts/
+-rw-r--r--   0 hsouchereau   (503) staff       (20)       80 2024-03-29 15:07:15.000000 galarp-0.0.5/galarp/hosts/__init__.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      880 2024-03-29 16:44:51.000000 galarp-0.0.5/galarp/hosts/densities.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     3200 2024-04-02 20:57:13.000000 galarp-0.0.5/galarp/hosts/hostorbits.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      264 2024-04-01 15:16:44.000000 galarp-0.0.5/galarp/hosts/initconditions.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     9502 2024-04-02 15:26:47.000000 galarp-0.0.5/galarp/particle_grids.py
+drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-06 17:11:23.539487 galarp-0.0.5/galarp/postprocessing/
+-rw-r--r--   0 hsouchereau   (503) staff       (20)       70 2024-04-01 22:01:07.000000 galarp-0.0.5/galarp/postprocessing/__init__.py
+drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-06 17:11:23.540079 galarp-0.0.5/galarp/postprocessing/plotting/
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      206 2024-04-03 14:34:47.000000 galarp-0.0.5/galarp/postprocessing/plotting/__init__.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     6382 2024-04-01 22:20:36.000000 galarp-0.0.5/galarp/postprocessing/plotting/general_plots.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     4212 2024-04-03 14:45:50.000000 galarp-0.0.5/galarp/postprocessing/plotting/matrix_plots.py
+drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-06 17:11:23.540367 galarp-0.0.5/galarp/postprocessing/plotting/tests/
+-rw-r--r--   0 hsouchereau   (503) staff       (20)        0 2024-04-02 14:01:03.000000 galarp-0.0.5/galarp/postprocessing/plotting/tests/__init__.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      656 2024-04-02 15:27:47.000000 galarp-0.0.5/galarp/postprocessing/plotting/tests/test_genplots.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     1753 2024-04-02 15:28:05.000000 galarp-0.0.5/galarp/postprocessing/plotting/utils.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     4734 2024-04-01 21:48:21.000000 galarp-0.0.5/galarp/postprocessing/utils.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     6420 2024-04-03 16:44:36.000000 galarp-0.0.5/galarp/rampressure.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     8030 2024-03-26 19:05:50.000000 galarp-0.0.5/galarp/shadows.py
+drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-06 17:11:23.541233 galarp-0.0.5/galarp/tests/
+-rw-r--r--   0 hsouchereau   (503) staff       (20)        0 2024-03-26 19:05:50.000000 galarp-0.0.5/galarp/tests/__init__.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      693 2024-04-01 16:19:47.000000 galarp-0.0.5/galarp/tests/helpers.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      747 2024-04-02 15:42:16.000000 galarp-0.0.5/galarp/tests/test_grids.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      519 2024-04-02 15:29:05.000000 galarp-0.0.5/galarp/tests/test_shadows.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     1201 2024-04-02 15:31:07.000000 galarp-0.0.5/galarp/tests/test_utils.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      732 2024-04-02 20:57:13.000000 galarp-0.0.5/galarp/tests/test_winds.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      659 2024-03-28 21:18:39.000000 galarp-0.0.5/galarp/tests.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     3435 2024-04-01 22:30:08.000000 galarp-0.0.5/galarp/utils.py
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     6762 2024-04-06 16:50:03.000000 galarp-0.0.5/galarp/winds.py
+drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-06 17:11:23.537412 galarp-0.0.5/galarp.egg-info/
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     1534 2024-04-06 17:11:23.000000 galarp-0.0.5/galarp.egg-info/PKG-INFO
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     1210 2024-04-06 17:11:23.000000 galarp-0.0.5/galarp.egg-info/SOURCES.txt
+-rw-r--r--   0 hsouchereau   (503) staff       (20)        1 2024-04-06 17:11:23.000000 galarp-0.0.5/galarp.egg-info/dependency_links.txt
+-rw-r--r--   0 hsouchereau   (503) staff       (20)       98 2024-04-06 17:11:23.000000 galarp-0.0.5/galarp.egg-info/requires.txt
+-rw-r--r--   0 hsouchereau   (503) staff       (20)        7 2024-04-06 17:11:23.000000 galarp-0.0.5/galarp.egg-info/top_level.txt
+-rw-r--r--   0 hsouchereau   (503) staff       (20)      617 2024-04-06 16:59:32.000000 galarp-0.0.5/pyproject.toml
+-rw-r--r--   0 hsouchereau   (503) staff       (20)       38 2024-04-06 17:11:23.541803 galarp-0.0.5/setup.cfg
+-rw-r--r--   0 hsouchereau   (503) staff       (20)     1309 2024-04-06 17:02:00.000000 galarp-0.0.5/setup.py
```

### Comparing `galarp-0.0.4/LICENSE` & `galarp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/PKG-INFO` & `galarp-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: galarp
-Version: 0.0.4
+Version: 0.0.5
 Summary: A ram pressure add-on for Gala numerical integration of gravitational potentials
 Home-page: https://github.com/HSouch/galarp
 Author: Harrison Souchereau
 Author-email: harrison.souchereau@yale.edu
 Keywords: galaxies,gravity,gravitational potentials
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gala
-Requires-Dist: astropy
-Requires-Dist: numpy
-Requires-Dist: matplotlib
+Requires-Dist: astropy>=6.0.0
+Requires-Dist: gala>=1.8.1
+Requires-Dist: k3d>=2.16.1
+Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: tqdm>=4.66.1
 
 GalaRP (`Gala <http://gala.adrian.pw/en/latest/>`_ + RP) is an analytical framework for gaseous evolution under ram pressure.
 
 |logo|
```

### Comparing `galarp-0.0.4/README.rst` & `galarp-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/__init__.py` & `galarp-0.0.5/galarp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 from .winds import *                # Classes for ram pressure wind
 
 from . import builtins
 
 from .hosts import *
 from .postprocessing import *
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

### Comparing `galarp-0.0.4/galarp/builtins/events.py` & `galarp-0.0.5/galarp/builtins/events.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/builtins/hosts.py` & `galarp-0.0.5/galarp/builtins/hosts.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/builtins/initconditions.py` & `galarp-0.0.5/galarp/builtins/initconditions.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/builtins/satellites.py` & `galarp-0.0.5/galarp/builtins/satellites.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/builtins/tests/test_builtins.py` & `galarp-0.0.5/galarp/builtins/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/hosts/densities.py` & `galarp-0.0.5/galarp/hosts/densities.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/hosts/hostorbits.py` & `galarp-0.0.5/galarp/hosts/hostorbits.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/particle_grids.py` & `galarp-0.0.5/galarp/particle_grids.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/postprocessing/plotting/general_plots.py` & `galarp-0.0.5/galarp/postprocessing/plotting/general_plots.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/postprocessing/plotting/matrix_plots.py` & `galarp-0.0.5/galarp/postprocessing/plotting/matrix_plots.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/postprocessing/plotting/tests/test_genplots.py` & `galarp-0.0.5/galarp/postprocessing/plotting/tests/test_genplots.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/postprocessing/plotting/utils.py` & `galarp-0.0.5/galarp/postprocessing/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/postprocessing/utils.py` & `galarp-0.0.5/galarp/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/rampressure.py` & `galarp-0.0.5/galarp/rampressure.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/shadows.py` & `galarp-0.0.5/galarp/shadows.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/tests/helpers.py` & `galarp-0.0.5/galarp/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/tests/test_grids.py` & `galarp-0.0.5/galarp/tests/test_grids.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/tests/test_shadows.py` & `galarp-0.0.5/galarp/tests/test_shadows.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/tests/test_utils.py` & `galarp-0.0.5/galarp/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/tests/test_winds.py` & `galarp-0.0.5/galarp/tests/test_winds.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/tests.py` & `galarp-0.0.5/galarp/tests.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/utils.py` & `galarp-0.0.5/galarp/utils.py`

 * *Files identical despite different names*

### Comparing `galarp-0.0.4/galarp/winds.py` & `galarp-0.0.5/galarp/winds.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 from astropy.table import Table
 import astropy.units as u
 from astropy.units import Quantity
 import numpy as np
 
+from gala.units import galactic
+
 from scipy.interpolate import interp1d
 
 
 
 __all__ = [
     "RPWind",
     "LorentzianWind",
@@ -120,48 +122,67 @@
 
     def evaluate(self, t):
         factor = t > self.t0
         return super().evaluate(t) * factor
     
 
 class InterpolatedWind(RPWind):
-    """ Wind class that returns an interpolated value for the wind vector at a given time t based on a scipy 
-        interp1D object.
+    """Wind that is interpolated from a table of values. """
 
-    """
-    def __init__(self, interp=None, inc=np.deg2rad(90), **kwargs):
+    def __init__(self, interp=None, units=galactic, **kwargs):
+        """
+            Args:
+                interp (callable): Interpolation function that takes a time value as input and returns the wind velocity at that time.
+                units (dict, optional): Dictionary specifying the units of the wind vector. Defaults to galactic units.
+                inc (float, optional): Inclination angle of the wind vector in radians. Defaults to 0.
+            """
         super().__init__(**kwargs)
-        self.inc = inc
-        self.vector = kwargs.get('vector', u.Quantity([np.cos(inc), 0, np.sin(inc)]) * u.km/u.s)
-
         self.interp = interp
+        self.inc = kwargs.get("inc", 0)
 
-        self.unit_vector = self.vector / np.linalg.norm(self.vector)
-        print(self.unit_vector)
-
-
+        self.unit_vector = [np.cos(self.inc), 0, np.sin(self.inc)]
+    
     def evaluate(self, t):
+        """ Evaluate the wind vector at a given time by multiplying the unit vector by the interpolated
+            wind strength at that time.
+        """
         return self.unit_vector * self.interp(t)
-    
-
-    def from_xy(self, xs, ys):
-        self.interp = interp1d(xs, ys, bounds_error=False, fill_value='extrapolate')
 
     @staticmethod
-    def from_table(fn, time_key, vel_keys, format='ascii', verbose=False, v_format=u.cm/u.s, ts_format=u.s, 
-                   **kwargs):
+    def from_table(fn, t_key, vel_keys, format="ascii",
+                   t_units = u.s, v_units = u.cm / u.s, 
+                   verbose=False, **kwargs):
+        """
+        Create an InterpolatedWind object from a table.
+
+        Parameters:
+        - fn (str): The filename of the table.
+        - t_key (str): The key for the time column in the table.
+        - vel_keys (str or list): The key(s) for the velocity column(s) in the table.
+        - format (str, optional): The format of the table. Default is "ascii".
+        - t_units (astropy.units.Unit, optional): The units for the time column. Default is u.s.
+        - v_units (astropy.units.Unit, optional): The units for the velocity column(s). Default is u.cm / u.s.
+        - verbose (bool, optional): Whether to print verbose output. Default is False.
+        - **kwargs: Additional keyword arguments to be passed to the InterpolatedWind constructor.
+
+        Returns:
+        - InterpolatedWind: An InterpolatedWind object created from the table.
+        Usage:
+                >>> wind = InterpolatedWind.from_table("wind_data.txt", "time", 
+                    ["velocity_x", "velocity_y", "velocity_z"], units=galactic, inc=np.deg2rad(45))
+                >>> print(wind.evaluate(10 * u.Myr))
+        """
         t = Table.read(fn, format=format)
 
         if verbose:
-            print(f'Loaded Table with {len(t)} rows, and keys: {t.keys()}')
+            print(f'Loaded table with {len(t)} rows and keys: {t.keys()}')
 
-        ts = t[time_key] * ts_format.to(u.Myr)
+        ts = t[t_key] * t_units.to(u.Myr)
 
-        if not isinstance(vel_keys, list): 
-            vel_keys = [vel_keys]
+        if not isinstance(vel_keys, list): vel_keys = [vel_keys]
 
         vels = np.array([t[key] for key in vel_keys])
-        v_tot = np.sqrt(np.sum(vels**2, axis=0)) * v_format
-        
-        interp = interp1d(ts, v_tot, bounds_error=False, fill_value='extrapolate')
+        v_tot = np.sqrt(np.sum(vels**2, axis=0)) * v_units.to(u.kpc/u.Myr)
+
+        interp = interp1d(ts, v_tot, bounds_error=False, fill_value="extrapolate")
 
         return InterpolatedWind(interp=interp, **kwargs)
```

### Comparing `galarp-0.0.4/galarp.egg-info/PKG-INFO` & `galarp-0.0.5/galarp.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: galarp
-Version: 0.0.4
+Version: 0.0.5
 Summary: A ram pressure add-on for Gala numerical integration of gravitational potentials
 Home-page: https://github.com/HSouch/galarp
 Author: Harrison Souchereau
 Author-email: harrison.souchereau@yale.edu
 Keywords: galaxies,gravity,gravitational potentials
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gala
-Requires-Dist: astropy
-Requires-Dist: numpy
-Requires-Dist: matplotlib
+Requires-Dist: astropy>=6.0.0
+Requires-Dist: gala>=1.8.1
+Requires-Dist: k3d>=2.16.1
+Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: tqdm>=4.66.1
 
 GalaRP (`Gala <http://gala.adrian.pw/en/latest/>`_ + RP) is an analytical framework for gaseous evolution under ram pressure.
 
 |logo|
```

### Comparing `galarp-0.0.4/galarp.egg-info/SOURCES.txt` & `galarp-0.0.5/galarp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

