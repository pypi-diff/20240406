# Comparing `tmp/shipper-shippy-2.33.2.tar.gz` & `tmp/shipper-shippy-2.33.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper-shippy-2.33.2.tar", last modified: Fri Apr  5 20:29:57 2024, max compression
+gzip compressed data, was "shipper-shippy-2.33.3.tar", last modified: Sat Apr  6 14:34:59 2024, max compression
```

## Comparing `shipper-shippy-2.33.2.tar` & `shipper-shippy-2.33.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:29:57.926961 shipper-shippy-2.33.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-05 20:29:57.926961 shipper-shippy-2.33.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:29:57.926961 shipper-shippy-2.33.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:29:57.926961 shipper-shippy-2.33.2/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:29:57.926961 shipper-shippy-2.33.2/shippy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:34:59.812360 shipper-shippy-2.33.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-06 14:34:59.812360 shipper-shippy-2.33.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 14:34:59.812360 shipper-shippy-2.33.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:34:59.812360 shipper-shippy-2.33.3/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-06 14:34:59.000000 shipper-shippy-2.33.3/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-06 14:34:59.000000 shipper-shippy-2.33.3/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:34:59.000000 shipper-shippy-2.33.3/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-06 14:34:59.000000 shipper-shippy-2.33.3/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-06 14:34:59.000000 shipper-shippy-2.33.3/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 14:34:59.000000 shipper-shippy-2.33.3/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:34:59.812360 shipper-shippy-2.33.3/shippy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-06 14:34:51.000000 shipper-shippy-2.33.3/shippy/version.py
```

### Comparing `shipper-shippy-2.33.2/PKG-INFO` & `shipper-shippy-2.33.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.33.2
+Version: 2.33.3
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: humanize==4.9.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: semver==3.0.2
-Requires-Dist: sentry-sdk==1.44.0
+Requires-Dist: sentry-sdk==1.44.1
 Requires-Dist: setuptools==69.2.0
 
 # shippy
 
 [
 ![PyPI](https://img.shields.io/pypi/v/shipper-shippy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/shipper-shippy)
```

### Comparing `shipper-shippy-2.33.2/README.md` & `shipper-shippy-2.33.3/README.md`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.2/setup.py` & `shipper-shippy-2.33.3/setup.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.2/shipper_shippy.egg-info/PKG-INFO` & `shipper-shippy-2.33.3/shipper_shippy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.33.2
+Version: 2.33.3
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: humanize==4.9.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: semver==3.0.2
-Requires-Dist: sentry-sdk==1.44.0
+Requires-Dist: sentry-sdk==1.44.1
 Requires-Dist: setuptools==69.2.0
 
 # shippy
 
 [
 ![PyPI](https://img.shields.io/pypi/v/shipper-shippy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/shipper-shippy)
```

### Comparing `shipper-shippy-2.33.2/shippy/__main__.py` & `shipper-shippy-2.33.3/shippy/__main__.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.2/shippy/client.py` & `shipper-shippy-2.33.3/shippy/client.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.2/shippy/config.py` & `shipper-shippy-2.33.3/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.2/shippy/constants.py` & `shipper-shippy-2.33.3/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.2/shippy/helper.py` & `shipper-shippy-2.33.3/shippy/helper.py`

 * *Files identical despite different names*

