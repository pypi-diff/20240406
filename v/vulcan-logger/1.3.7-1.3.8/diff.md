# Comparing `tmp/vulcan-logger-1.3.7.tar.gz` & `tmp/vulcan-logger-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.3.7.tar", last modified: Sat Apr  6 20:53:21 2024, max compression
+gzip compressed data, was "vulcan-logger-1.3.8.tar", last modified: Sat Apr  6 20:57:13 2024, max compression
```

## Comparing `vulcan-logger-1.3.7.tar` & `vulcan-logger-1.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:53:21.759084 vulcan-logger-1.3.7/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-06 20:53:21.759084 vulcan-logger-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:53:21.759084 vulcan-logger-1.3.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:53:21.755084 vulcan-logger-1.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/tests/test_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5513 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:53:21.759084 vulcan-logger-1.3.7/vulcan_logger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/vulcan_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/vulcan_logger/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/vulcan_logger/encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4152 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/vulcan_logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:53:21.759084 vulcan-logger-1.3.7/vulcan_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-06 20:53:21.000000 vulcan-logger-1.3.7/vulcan_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 20:53:21.000000 vulcan-logger-1.3.7/vulcan_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:53:21.000000 vulcan-logger-1.3.7/vulcan_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 20:53:21.000000 vulcan-logger-1.3.7/vulcan_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-06 20:53:21.000000 vulcan-logger-1.3.7/vulcan_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:57:13.785175 vulcan-logger-1.3.8/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-06 20:57:00.000000 vulcan-logger-1.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-06 20:57:13.785175 vulcan-logger-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:57:13.785175 vulcan-logger-1.3.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-06 20:57:00.000000 vulcan-logger-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:57:13.785175 vulcan-logger-1.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-06 20:57:00.000000 vulcan-logger-1.3.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-06 20:57:00.000000 vulcan-logger-1.3.8/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-06 20:57:00.000000 vulcan-logger-1.3.8/tests/test_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5513 2024-04-06 20:57:00.000000 vulcan-logger-1.3.8/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:57:13.785175 vulcan-logger-1.3.8/vulcan_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-06 20:57:00.000000 vulcan-logger-1.3.8/vulcan_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-06 20:57:00.000000 vulcan-logger-1.3.8/vulcan_logger/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-06 20:57:00.000000 vulcan-logger-1.3.8/vulcan_logger/encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4152 2024-04-06 20:57:00.000000 vulcan-logger-1.3.8/vulcan_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:57:13.785175 vulcan-logger-1.3.8/vulcan_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-06 20:57:13.000000 vulcan-logger-1.3.8/vulcan_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 20:57:13.000000 vulcan-logger-1.3.8/vulcan_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:57:13.000000 vulcan-logger-1.3.8/vulcan_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 20:57:13.000000 vulcan-logger-1.3.8/vulcan_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-06 20:57:13.000000 vulcan-logger-1.3.8/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.3.7/LICENSE` & `vulcan-logger-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.7/PKG-INFO` & `vulcan-logger-1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.3.7
+Version: 1.3.8
 Summary: A logging utility package with colored logs.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vulcan-logger-1.3.7/tests/test_decorator.py` & `vulcan-logger-1.3.8/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.7/tests/test_encoder.py` & `vulcan-logger-1.3.8/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.7/tests/test_logger.py` & `vulcan-logger-1.3.8/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.7/vulcan_logger/decorator.py` & `vulcan-logger-1.3.8/vulcan_logger/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.7/vulcan_logger/encoder.py` & `vulcan-logger-1.3.8/vulcan_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.7/vulcan_logger/logger.py` & `vulcan-logger-1.3.8/vulcan_logger/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.7/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.3.8/vulcan_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.3.7
+Version: 1.3.8
 Summary: A logging utility package with colored logs.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

