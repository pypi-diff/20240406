# Comparing `tmp/medusa-logger-1.0.4.tar.gz` & `tmp/medusa-logger-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medusa-logger-1.0.4.tar", last modified: Sat Apr  6 16:59:32 2024, max compression
+gzip compressed data, was "medusa-logger-1.0.5.tar", last modified: Sat Apr  6 17:02:20 2024, max compression
```

## Comparing `medusa-logger-1.0.4.tar` & `medusa-logger-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 16:59:32.264231 medusa-logger-1.0.4/
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)     1070 2024-04-05 16:36:38.000000 medusa-logger-1.0.4/LICENSE
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2514 2024-04-06 16:59:32.264231 medusa-logger-1.0.4/PKG-INFO
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 16:59:32.264231 medusa-logger-1.0.4/example/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        0 2024-04-06 15:39:29.000000 medusa-logger-1.0.4/example/__init__.py
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)     1464 2024-04-06 16:22:30.000000 medusa-logger-1.0.4/example/example.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 16:59:32.264231 medusa-logger-1.0.4/medusa_logger/
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)       41 2024-04-06 16:22:42.000000 medusa-logger-1.0.4/medusa_logger/__init__.py
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)     3677 2024-04-06 06:46:18.000000 medusa-logger-1.0.4/medusa_logger/decorator.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1529 2024-04-06 06:49:50.000000 medusa-logger-1.0.4/medusa_logger/encoder.py
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)     4152 2024-04-06 04:36:41.000000 medusa-logger-1.0.4/medusa_logger/logger.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 16:59:32.264231 medusa-logger-1.0.4/medusa_logger.egg-info/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2514 2024-04-06 16:59:32.000000 medusa-logger-1.0.4/medusa_logger.egg-info/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      426 2024-04-06 16:59:32.000000 medusa-logger-1.0.4/medusa_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2024-04-06 16:59:32.000000 medusa-logger-1.0.4/medusa_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       12 2024-04-06 16:59:32.000000 medusa-logger-1.0.4/medusa_logger.egg-info/requires.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       28 2024-04-06 16:59:32.000000 medusa-logger-1.0.4/medusa_logger.egg-info/top_level.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2024-04-06 16:59:32.264231 medusa-logger-1.0.4/setup.cfg
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)      402 2024-04-06 16:59:31.000000 medusa-logger-1.0.4/setup.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 16:59:32.264231 medusa-logger-1.0.4/tests/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       56 2024-04-06 04:57:59.000000 medusa-logger-1.0.4/tests/__init__.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2401 2024-04-06 05:38:53.000000 medusa-logger-1.0.4/tests/test_decorator.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2144 2024-04-06 05:42:53.000000 medusa-logger-1.0.4/tests/test_encoder.py
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)     5513 2024-04-06 05:54:38.000000 medusa-logger-1.0.4/tests/test_logger.py
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 17:02:20.378543 medusa-logger-1.0.5/
+-rwxrwxrwx   0 jacob     (1000) jacob     (1000)     1070 2024-04-05 16:36:38.000000 medusa-logger-1.0.5/LICENSE
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     2551 2024-04-06 17:02:20.374543 medusa-logger-1.0.5/PKG-INFO
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 17:02:20.374543 medusa-logger-1.0.5/example/
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)        0 2024-04-06 15:39:29.000000 medusa-logger-1.0.5/example/__init__.py
+-rwxrwxrwx   0 jacob     (1000) jacob     (1000)     1464 2024-04-06 16:22:30.000000 medusa-logger-1.0.5/example/example.py
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 17:02:20.374543 medusa-logger-1.0.5/medusa_logger/
+-rwxrwxrwx   0 jacob     (1000) jacob     (1000)       41 2024-04-06 16:22:42.000000 medusa-logger-1.0.5/medusa_logger/__init__.py
+-rwxrwxrwx   0 jacob     (1000) jacob     (1000)     3677 2024-04-06 06:46:18.000000 medusa-logger-1.0.5/medusa_logger/decorator.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     1529 2024-04-06 06:49:50.000000 medusa-logger-1.0.5/medusa_logger/encoder.py
+-rwxrwxrwx   0 jacob     (1000) jacob     (1000)     4152 2024-04-06 04:36:41.000000 medusa-logger-1.0.5/medusa_logger/logger.py
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 17:02:20.374543 medusa-logger-1.0.5/medusa_logger.egg-info/
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     2551 2024-04-06 17:02:20.000000 medusa-logger-1.0.5/medusa_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)      426 2024-04-06 17:02:20.000000 medusa-logger-1.0.5/medusa_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2024-04-06 17:02:20.000000 medusa-logger-1.0.5/medusa_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       12 2024-04-06 17:02:20.000000 medusa-logger-1.0.5/medusa_logger.egg-info/requires.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       28 2024-04-06 17:02:20.000000 medusa-logger-1.0.5/medusa_logger.egg-info/top_level.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2024-04-06 17:02:20.378543 medusa-logger-1.0.5/setup.cfg
+-rwxrwxrwx   0 jacob     (1000) jacob     (1000)      400 2024-04-06 17:02:20.000000 medusa-logger-1.0.5/setup.py
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 17:02:20.374543 medusa-logger-1.0.5/tests/
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       56 2024-04-06 04:57:59.000000 medusa-logger-1.0.5/tests/__init__.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     2401 2024-04-06 05:38:53.000000 medusa-logger-1.0.5/tests/test_decorator.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     2144 2024-04-06 05:42:53.000000 medusa-logger-1.0.5/tests/test_encoder.py
+-rwxrwxrwx   0 jacob     (1000) jacob     (1000)     5513 2024-04-06 05:54:38.000000 medusa-logger-1.0.5/tests/test_logger.py
```

### Comparing `medusa-logger-1.0.4/LICENSE` & `medusa-logger-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.0.4/PKG-INFO` & `medusa-logger-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: medusa-logger
-Version: 1.0.4
-Summary: UNKNOWN
+Version: 1.0.5
+Summary: A logging utility package with colored logs.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Medusa Logger
```

### Comparing `medusa-logger-1.0.4/example/example.py` & `medusa-logger-1.0.5/example/example.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.0.4/medusa_logger/decorator.py` & `medusa-logger-1.0.5/medusa_logger/decorator.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.0.4/medusa_logger/encoder.py` & `medusa-logger-1.0.5/medusa_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.0.4/medusa_logger/logger.py` & `medusa-logger-1.0.5/medusa_logger/logger.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.0.4/medusa_logger.egg-info/PKG-INFO` & `medusa-logger-1.0.5/medusa_logger.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: medusa-logger
-Version: 1.0.4
-Summary: UNKNOWN
+Version: 1.0.5
+Summary: A logging utility package with colored logs.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Medusa Logger
```

### Comparing `medusa-logger-1.0.4/tests/test_decorator.py` & `medusa-logger-1.0.5/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.0.4/tests/test_encoder.py` & `medusa-logger-1.0.5/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.0.4/tests/test_logger.py` & `medusa-logger-1.0.5/tests/test_logger.py`

 * *Files identical despite different names*
