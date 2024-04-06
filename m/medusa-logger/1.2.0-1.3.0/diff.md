# Comparing `tmp/medusa-logger-1.2.0.tar.gz` & `tmp/medusa-logger-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medusa-logger-1.2.0.tar", last modified: Sat Apr  6 17:53:06 2024, max compression
+gzip compressed data, was "medusa-logger-1.3.0.tar", last modified: Sat Apr  6 18:32:46 2024, max compression
```

## Comparing `medusa-logger-1.2.0.tar` & `medusa-logger-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 17:53:06.951770 medusa-logger-1.2.0/
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)     1070 2024-04-05 16:36:38.000000 medusa-logger-1.2.0/LICENSE
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     4266 2024-04-06 17:53:06.951770 medusa-logger-1.2.0/PKG-INFO
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 17:53:06.951770 medusa-logger-1.2.0/example/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        0 2024-04-06 15:39:29.000000 medusa-logger-1.2.0/example/__init__.py
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)     1464 2024-04-06 16:22:30.000000 medusa-logger-1.2.0/example/example.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 17:53:06.951770 medusa-logger-1.2.0/medusa_logger/
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)       41 2024-04-06 16:22:42.000000 medusa-logger-1.2.0/medusa_logger/__init__.py
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)     3677 2024-04-06 06:46:18.000000 medusa-logger-1.2.0/medusa_logger/decorator.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1529 2024-04-06 06:49:50.000000 medusa-logger-1.2.0/medusa_logger/encoder.py
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)     4152 2024-04-06 04:36:41.000000 medusa-logger-1.2.0/medusa_logger/logger.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 17:53:06.951770 medusa-logger-1.2.0/medusa_logger.egg-info/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     4266 2024-04-06 17:53:06.000000 medusa-logger-1.2.0/medusa_logger.egg-info/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      426 2024-04-06 17:53:06.000000 medusa-logger-1.2.0/medusa_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2024-04-06 17:53:06.000000 medusa-logger-1.2.0/medusa_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       12 2024-04-06 17:53:06.000000 medusa-logger-1.2.0/medusa_logger.egg-info/requires.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       28 2024-04-06 17:53:06.000000 medusa-logger-1.2.0/medusa_logger.egg-info/top_level.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2024-04-06 17:53:06.951770 medusa-logger-1.2.0/setup.cfg
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)      400 2024-04-06 17:53:06.000000 medusa-logger-1.2.0/setup.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-06 17:53:06.951770 medusa-logger-1.2.0/tests/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       56 2024-04-06 04:57:59.000000 medusa-logger-1.2.0/tests/__init__.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2401 2024-04-06 05:38:53.000000 medusa-logger-1.2.0/tests/test_decorator.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2144 2024-04-06 05:42:53.000000 medusa-logger-1.2.0/tests/test_encoder.py
--rwxrwxrwx   0 jacob     (1000) jacob     (1000)     5513 2024-04-06 05:54:38.000000 medusa-logger-1.2.0/tests/test_logger.py
+drwxrwxr-x   0 medusa    (1001) medusa    (1001)        0 2024-04-06 18:32:46.072486 medusa-logger-1.3.0/
+-rwxrwxr-x   0 medusa    (1001) medusa    (1001)     1070 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/LICENSE
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)     4302 2024-04-06 18:32:46.072486 medusa-logger-1.3.0/PKG-INFO
+drwxrwxr-x   0 medusa    (1001) medusa    (1001)        0 2024-04-06 18:32:46.072486 medusa-logger-1.3.0/example/
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)        0 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/example/__init__.py
+-rwxrwxr-x   0 medusa    (1001) medusa    (1001)     1223 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/example/example.py
+drwxrwxr-x   0 medusa    (1001) medusa    (1001)        0 2024-04-06 18:32:46.072486 medusa-logger-1.3.0/medusa_logger/
+-rwxrwxr-x   0 medusa    (1001) medusa    (1001)       41 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/medusa_logger/__init__.py
+-rwxrwxr-x   0 medusa    (1001) medusa    (1001)     3677 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/medusa_logger/decorator.py
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)     1529 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/medusa_logger/encoder.py
+-rwxrwxr-x   0 medusa    (1001) medusa    (1001)     4152 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/medusa_logger/logger.py
+drwxrwxr-x   0 medusa    (1001) medusa    (1001)        0 2024-04-06 18:32:46.072486 medusa-logger-1.3.0/medusa_logger.egg-info/
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)     4302 2024-04-06 18:32:46.000000 medusa-logger-1.3.0/medusa_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)      426 2024-04-06 18:32:46.000000 medusa-logger-1.3.0/medusa_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)        1 2024-04-06 18:32:46.000000 medusa-logger-1.3.0/medusa_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)       12 2024-04-06 18:32:46.000000 medusa-logger-1.3.0/medusa_logger.egg-info/requires.txt
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)       28 2024-04-06 18:32:46.000000 medusa-logger-1.3.0/medusa_logger.egg-info/top_level.txt
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)       38 2024-04-06 18:32:46.072486 medusa-logger-1.3.0/setup.cfg
+-rwxrwxr-x   0 medusa    (1001) medusa    (1001)      400 2024-04-06 18:32:45.000000 medusa-logger-1.3.0/setup.py
+drwxrwxr-x   0 medusa    (1001) medusa    (1001)        0 2024-04-06 18:32:46.072486 medusa-logger-1.3.0/tests/
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)       56 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/tests/__init__.py
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)     2401 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/tests/test_decorator.py
+-rw-rw-r--   0 medusa    (1001) medusa    (1001)     2144 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/tests/test_encoder.py
+-rwxrwxr-x   0 medusa    (1001) medusa    (1001)     5513 2024-04-06 18:05:29.000000 medusa-logger-1.3.0/tests/test_logger.py
```

### Comparing `medusa-logger-1.2.0/LICENSE` & `medusa-logger-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.2.0/PKG-INFO` & `medusa-logger-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: medusa-logger
-Version: 1.2.0
+Version: 1.3.0
 Summary: A logging utility package with colored logs.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Medusa Logger
 Medusa Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
 
 [View the full documentation here](https://medusa-logger.readthedocs.io/en/latest/)
 
+![Medusa Logger](img/examples.png)
+
 ## Features
 - **Caller Information**: Automatically includes the caller's filename and line number in log messages for better traceability.
 - **Customizable Log Levels**: Easily configure log levels to control the severity of messages that the logger will process.
 - **Colored Logs**: Enhance log readability with colored logs for different log levels.
 - **Conditional Logging**: Conditionally log messages based on specific conditions to control verbosity.
 
 ## Installation
```

### Comparing `medusa-logger-1.2.0/example/example.py` & `medusa-logger-1.3.0/example/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 # example/example.py
-import sys
 import os
-# Manual sys path update for package imports, so this file can be used
-# without PIP installing the package.
-from pathlib import Path
-sys.path.append(str(Path(__file__).resolve().parent.parent))
-try:
-    from medusa_logger.logger import Logger
-    from medusa_logger.decorator import log
-except:
-    sys.exit(1)
+
+from medusa_logger.logger import Logger
+from medusa_logger.decorator import log
+
 
 os.environ["MD_LOG_LEVEL"] = "DEBUG"  # Global log level filter
 
 # Functions defined with a log decorator. Level or Condition may be
 # passed as arguments on the decorator, or omitted.
```

### Comparing `medusa-logger-1.2.0/medusa_logger/decorator.py` & `medusa-logger-1.3.0/medusa_logger/decorator.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.2.0/medusa_logger/encoder.py` & `medusa-logger-1.3.0/medusa_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.2.0/medusa_logger/logger.py` & `medusa-logger-1.3.0/medusa_logger/logger.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.2.0/medusa_logger.egg-info/PKG-INFO` & `medusa-logger-1.3.0/medusa_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: medusa-logger
-Version: 1.2.0
+Version: 1.3.0
 Summary: A logging utility package with colored logs.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Medusa Logger
 Medusa Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
 
 [View the full documentation here](https://medusa-logger.readthedocs.io/en/latest/)
 
+![Medusa Logger](img/examples.png)
+
 ## Features
 - **Caller Information**: Automatically includes the caller's filename and line number in log messages for better traceability.
 - **Customizable Log Levels**: Easily configure log levels to control the severity of messages that the logger will process.
 - **Colored Logs**: Enhance log readability with colored logs for different log levels.
 - **Conditional Logging**: Conditionally log messages based on specific conditions to control verbosity.
 
 ## Installation
```

### Comparing `medusa-logger-1.2.0/tests/test_decorator.py` & `medusa-logger-1.3.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.2.0/tests/test_encoder.py` & `medusa-logger-1.3.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `medusa-logger-1.2.0/tests/test_logger.py` & `medusa-logger-1.3.0/tests/test_logger.py`

 * *Files identical despite different names*

