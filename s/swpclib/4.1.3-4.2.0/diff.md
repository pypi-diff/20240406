# Comparing `tmp/swpclib-4.1.3.tar.gz` & `tmp/swpclib-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swpclib-4.1.3.tar", last modified: Fri Apr  5 03:30:57 2024, max compression
+gzip compressed data, was "swpclib-4.2.0.tar", last modified: Sat Apr  6 04:33:35 2024, max compression
```

## Comparing `swpclib-4.1.3.tar` & `swpclib-4.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:30:57.586815 swpclib-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-05 03:30:47.000000 swpclib-4.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 03:30:47.000000 swpclib-4.1.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 03:30:47.000000 swpclib-4.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-05 03:30:47.000000 swpclib-4.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-05 03:30:57.586815 swpclib-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 03:30:47.000000 swpclib-4.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:30:57.586815 swpclib-4.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-05 03:30:47.000000 swpclib-4.1.3/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-05 03:30:47.000000 swpclib-4.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 03:30:47.000000 swpclib-4.1.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 03:30:47.000000 swpclib-4.1.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-05 03:30:47.000000 swpclib-4.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 03:30:47.000000 swpclib-4.1.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 03:30:47.000000 swpclib-4.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 03:30:47.000000 swpclib-4.1.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 03:30:47.000000 swpclib-4.1.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-05 03:30:47.000000 swpclib-4.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 03:30:57.586815 swpclib-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-05 03:30:47.000000 swpclib-4.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:30:57.586815 swpclib-4.1.3/swpclib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 03:30:47.000000 swpclib-4.1.3/swpclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-05 03:30:47.000000 swpclib-4.1.3/swpclib/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-05 03:30:47.000000 swpclib-4.1.3/swpclib/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-05 03:30:47.000000 swpclib-4.1.3/swpclib/swpclib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:30:57.586815 swpclib-4.1.3/swpclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-05 03:30:57.000000 swpclib-4.1.3/swpclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-05 03:30:57.000000 swpclib-4.1.3/swpclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:30:57.000000 swpclib-4.1.3/swpclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 03:30:57.000000 swpclib-4.1.3/swpclib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 03:30:57.000000 swpclib-4.1.3/swpclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 03:30:57.000000 swpclib-4.1.3/swpclib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:30:57.586815 swpclib-4.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 03:30:47.000000 swpclib-4.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-05 03:30:47.000000 swpclib-4.1.3/tests/test_swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:33:35.356449 swpclib-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-06 04:33:26.000000 swpclib-4.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-06 04:33:26.000000 swpclib-4.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 04:33:26.000000 swpclib-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-06 04:33:26.000000 swpclib-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-06 04:33:35.356449 swpclib-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 04:33:26.000000 swpclib-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:33:35.352449 swpclib-4.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-06 04:33:26.000000 swpclib-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-06 04:33:35.356449 swpclib-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-06 04:33:26.000000 swpclib-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:33:35.352449 swpclib-4.2.0/swpclib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-06 04:33:26.000000 swpclib-4.2.0/swpclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-06 04:33:26.000000 swpclib-4.2.0/swpclib/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-06 04:33:26.000000 swpclib-4.2.0/swpclib/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-06 04:33:26.000000 swpclib-4.2.0/swpclib/swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:33:35.356449 swpclib-4.2.0/swpclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:33:35.356449 swpclib-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-06 04:33:26.000000 swpclib-4.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-06 04:33:26.000000 swpclib-4.2.0/tests/test_swpclib.py
```

### Comparing `swpclib-4.1.3/CONTRIBUTING.rst` & `swpclib-4.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.1.3/LICENSE` & `swpclib-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swpclib-4.1.3/docs/Makefile` & `swpclib-4.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swpclib-4.1.3/docs/conf.py` & `swpclib-4.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.1.3/docs/installation.rst` & `swpclib-4.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.1.3/docs/make.bat` & `swpclib-4.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swpclib-4.1.3/setup.py` & `swpclib-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.1.3/swpclib/alerts.py` & `swpclib-4.2.0/swpclib/alerts.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.1.3/swpclib/cli.py` & `swpclib-4.2.0/swpclib/cli.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.1.3/swpclib/swpclib.py` & `swpclib-4.2.0/swpclib/swpclib.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         return ssn_data
 
     async def get_kp(self, start=0, end=1, step=1):
         """get planetary k index"""
 
         try:
             data = await self.get_data_method("json/planetary_k_index_1m.json")
+            data.reverse()
             data_range = slice(start, end, step)
             kp_data = {
                 "kp_index_data": {
                     "kp_index": float(item["kp_index"]),
                     "timestamp": item["time_tag"],
                 }
                 for item in data[data_range]
```

### Comparing `swpclib-4.1.3/swpclib.egg-info/SOURCES.txt` & `swpclib-4.2.0/swpclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swpclib-4.1.3/tests/test_swpclib.py` & `swpclib-4.2.0/tests/test_swpclib.py`

 * *Files identical despite different names*

