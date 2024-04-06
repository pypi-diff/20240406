# Comparing `tmp/vulcan-logger-1.3.6.tar.gz` & `tmp/vulcan-logger-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.3.6.tar", last modified: Sat Apr  6 19:58:35 2024, max compression
+gzip compressed data, was "vulcan-logger-1.3.7.tar", last modified: Sat Apr  6 20:53:21 2024, max compression
```

## Comparing `vulcan-logger-1.3.6.tar` & `vulcan-logger-1.3.7.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:58:35.389292 vulcan-logger-1.3.6/
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     1070 2024-04-06 19:41:05.000000 vulcan-logger-1.3.6/LICENSE
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     4492 2024-04-06 19:58:35.389292 vulcan-logger-1.3.6/PKG-INFO
-drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:58:35.385292 vulcan-logger-1.3.6/example/
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     1223 2024-04-06 19:49:59.000000 vulcan-logger-1.3.6/example/example.py
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       38 2024-04-06 19:58:35.389292 vulcan-logger-1.3.6/setup.cfg
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)      400 2024-04-06 19:58:35.000000 vulcan-logger-1.3.6/setup.py
-drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:58:35.385292 vulcan-logger-1.3.6/tests/
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       56 2024-04-06 19:41:05.000000 vulcan-logger-1.3.6/tests/__init__.py
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     2401 2024-04-06 19:50:13.000000 vulcan-logger-1.3.6/tests/test_decorator.py
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     2144 2024-04-06 19:53:52.000000 vulcan-logger-1.3.6/tests/test_encoder.py
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     5513 2024-04-06 19:50:20.000000 vulcan-logger-1.3.6/tests/test_logger.py
-drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:58:35.385292 vulcan-logger-1.3.6/vulcan_logger/
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)       41 2024-04-06 19:41:05.000000 vulcan-logger-1.3.6/vulcan_logger/__init__.py
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     3677 2024-04-06 19:41:05.000000 vulcan-logger-1.3.6/vulcan_logger/decorator.py
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     1529 2024-04-06 19:41:05.000000 vulcan-logger-1.3.6/vulcan_logger/encoder.py
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     4152 2024-04-06 19:41:05.000000 vulcan-logger-1.3.6/vulcan_logger/logger.py
-drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:58:35.389292 vulcan-logger-1.3.6/vulcan_logger.egg-info/
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     4492 2024-04-06 19:58:35.000000 vulcan-logger-1.3.6/vulcan_logger.egg-info/PKG-INFO
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)      406 2024-04-06 19:58:35.000000 vulcan-logger-1.3.6/vulcan_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)        1 2024-04-06 19:58:35.000000 vulcan-logger-1.3.6/vulcan_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       12 2024-04-06 19:58:35.000000 vulcan-logger-1.3.6/vulcan_logger.egg-info/requires.txt
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       20 2024-04-06 19:58:35.000000 vulcan-logger-1.3.6/vulcan_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:53:21.759084 vulcan-logger-1.3.7/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-06 20:53:21.759084 vulcan-logger-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:53:21.759084 vulcan-logger-1.3.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:53:21.755084 vulcan-logger-1.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/tests/test_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5513 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:53:21.759084 vulcan-logger-1.3.7/vulcan_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/vulcan_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/vulcan_logger/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/vulcan_logger/encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4152 2024-04-06 20:53:12.000000 vulcan-logger-1.3.7/vulcan_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:53:21.759084 vulcan-logger-1.3.7/vulcan_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-06 20:53:21.000000 vulcan-logger-1.3.7/vulcan_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 20:53:21.000000 vulcan-logger-1.3.7/vulcan_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:53:21.000000 vulcan-logger-1.3.7/vulcan_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 20:53:21.000000 vulcan-logger-1.3.7/vulcan_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-06 20:53:21.000000 vulcan-logger-1.3.7/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.3.6/LICENSE` & `vulcan-logger-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.6/PKG-INFO` & `vulcan-logger-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.3.6
+Version: 1.3.7
 Summary: A logging utility package with colored logs.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vulcan-logger-1.3.6/tests/test_decorator.py` & `vulcan-logger-1.3.7/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.6/tests/test_encoder.py` & `vulcan-logger-1.3.7/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.6/tests/test_logger.py` & `vulcan-logger-1.3.7/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.6/vulcan_logger/decorator.py` & `vulcan-logger-1.3.7/vulcan_logger/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.6/vulcan_logger/encoder.py` & `vulcan-logger-1.3.7/vulcan_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.6/vulcan_logger/logger.py` & `vulcan-logger-1.3.7/vulcan_logger/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.6/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.3.7/vulcan_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.3.6
+Version: 1.3.7
 Summary: A logging utility package with colored logs.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

