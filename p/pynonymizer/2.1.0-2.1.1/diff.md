# Comparing `tmp/pynonymizer-2.1.0.tar.gz` & `tmp/pynonymizer-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynonymizer-2.1.0.tar", last modified: Wed Apr  3 13:39:48 2024, max compression
+gzip compressed data, was "pynonymizer-2.1.1.tar", last modified: Sat Apr  6 14:12:39 2024, max compression
```

## Comparing `pynonymizer-2.1.0.tar` & `pynonymizer-2.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     1050 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6570 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5717 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.991476 pynonymizer-2.1.0/pynonymizer/
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/__main__.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.995477 pynonymizer-2.1.0/pynonymizer/database/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2791 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.995477 pynonymizer-2.1.0/pynonymizer/database/mssql/
--rw-r--r--   0 root         (0) root         (0)    16622 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8518 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/mssql/connectionstring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.995477 pynonymizer-2.1.0/pynonymizer/database/mysql/
--rw-r--r--   0 root         (0) root         (0)     7478 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5214 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/mysql/execution.py
--rw-r--r--   0 root         (0) root         (0)     4560 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/mysql/query_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.995477 pynonymizer-2.1.0/pynonymizer/database/postgres/
--rw-r--r--   0 root         (0) root         (0)     7321 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4305 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/postgres/execution.py
--rw-r--r--   0 root         (0) root         (0)     5252 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/postgres/query_factory.py
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/provider.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.995477 pynonymizer-2.1.0/pynonymizer/fake/
--rw-r--r--   0 root         (0) root         (0)     3823 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/fake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3848 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/process_steps.py
--rw-r--r--   0 root         (0) root         (0)     4750 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/pynonymize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/pynonymizer/strategy/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      543 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/config.py
--rw-r--r--   0 root         (0) root         (0)     1910 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/database.py
--rw-r--r--   0 root         (0) root         (0)      797 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8132 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/parser.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/table.py
--rw-r--r--   0 root         (0) root         (0)     3283 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/update_column.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/pynonymizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6570 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1144 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      122 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1235 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)      462 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/tests/test_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6537 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5684 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.817706 pynonymizer-2.1.1/pynonymizer/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.821706 pynonymizer-2.1.1/pynonymizer/database/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.821706 pynonymizer-2.1.1/pynonymizer/database/mssql/
+-rw-r--r--   0 root         (0) root         (0)    16622 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8518 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/mssql/connectionstring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.821706 pynonymizer-2.1.1/pynonymizer/database/mysql/
+-rw-r--r--   0 root         (0) root         (0)     7478 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5214 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/mysql/execution.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/mysql/query_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.821706 pynonymizer-2.1.1/pynonymizer/database/postgres/
+-rw-r--r--   0 root         (0) root         (0)     7321 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/postgres/execution.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/postgres/query_factory.py
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/provider.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.821706 pynonymizer-2.1.1/pynonymizer/fake/
+-rw-r--r--   0 root         (0) root         (0)     3823 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/fake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/process_steps.py
+-rw-r--r--   0 root         (0) root         (0)     4750 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/pynonymize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/pynonymizer/strategy/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      543 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/config.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/database.py
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8132 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/table.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/update_column.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/pynonymizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6537 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      462 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/tests/test_meta.py
```

### Comparing `pynonymizer-2.1.0/LICENSE` & `pynonymizer-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/PKG-INFO` & `pynonymizer-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynonymizer
-Version: 2.1.0
+Version: 2.1.1
 Summary: An anonymization tool for production databases
 Home-page: https://github.com/rwnx/pynonymizer
 Author: Rowan Twell
 Author-email: rowantwell@gmail.com
 License: MIT
 Keywords: anonymization gdpr database mysql
 Classifier: Development Status :: 5 - Production/Stable
@@ -80,17 +80,14 @@
 1. Restore from dumpfile to temporary database.
 1. Anonymize temporary database with strategy.
 1. Dump resulting data to file.
 1. Drop temporary database.
 
 If this workflow doesnt work for you, see [process control](https://github.com/rwnx/pynonymizer/blob/main/doc/process-control.md) to see if it can be adjusted to suit your needs.
 
-## Requirements
-* Python >= 3.6
-
 ### mysql
 * `mysql`/`mysqldump` Must be in $PATH
 * Local or remote mysql >= 5.5
 * Supported Inputs:
   * Plain SQL over stdout
   * Plain SQL file `.sql`
   * GZip-compressed SQL file `.gz`
```

### Comparing `pynonymizer-2.1.0/README.md` & `pynonymizer-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,14 @@
 1. Restore from dumpfile to temporary database.
 1. Anonymize temporary database with strategy.
 1. Dump resulting data to file.
 1. Drop temporary database.
 
 If this workflow doesnt work for you, see [process control](https://github.com/rwnx/pynonymizer/blob/main/doc/process-control.md) to see if it can be adjusted to suit your needs.
 
-## Requirements
-* Python >= 3.6
-
 ### mysql
 * `mysql`/`mysqldump` Must be in $PATH
 * Local or remote mysql >= 5.5
 * Supported Inputs:
   * Plain SQL over stdout
   * Plain SQL file `.sql`
   * GZip-compressed SQL file `.gz`
```

### Comparing `pynonymizer-2.1.0/pynonymizer/cli.py` & `pynonymizer-2.1.1/pynonymizer/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             "--start-at", help="Choose a step to begin the process (inclusive)."
         ),
     ] = "START",
     only_step: Annotated[str, typer.Option(help="Choose one step to perform.")] = None,
     skip_steps: Annotated[
         List[str],
         typer.Option(
-            "--skip_steps",
+            "--skip-steps",
             show_envvar=True,
             help="Choose one or more steps to skip",
             case_sensitive=False,
         ),
     ] = None,
     stop_at_step: Annotated[
         str,
```

### Comparing `pynonymizer-2.1.0/pynonymizer/database/exceptions.py` & `pynonymizer-2.1.1/pynonymizer/database/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/database/io.py` & `pynonymizer-2.1.1/pynonymizer/database/io.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/database/mssql/__init__.py` & `pynonymizer-2.1.1/pynonymizer/database/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/database/mssql/connectionstring.py` & `pynonymizer-2.1.1/pynonymizer/database/mssql/connectionstring.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/database/mysql/__init__.py` & `pynonymizer-2.1.1/pynonymizer/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/database/mysql/execution.py` & `pynonymizer-2.1.1/pynonymizer/database/mysql/execution.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/database/mysql/query_factory.py` & `pynonymizer-2.1.1/pynonymizer/database/mysql/query_factory.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/database/postgres/__init__.py` & `pynonymizer-2.1.1/pynonymizer/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/database/postgres/execution.py` & `pynonymizer-2.1.1/pynonymizer/database/postgres/execution.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/database/postgres/query_factory.py` & `pynonymizer-2.1.1/pynonymizer/database/postgres/query_factory.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/fake/__init__.py` & `pynonymizer-2.1.1/pynonymizer/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/process_steps.py` & `pynonymizer-2.1.1/pynonymizer/process_steps.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/pynonymize.py` & `pynonymizer-2.1.1/pynonymizer/pynonymize.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/strategy/config.py` & `pynonymizer-2.1.1/pynonymizer/strategy/config.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/strategy/database.py` & `pynonymizer-2.1.1/pynonymizer/strategy/database.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/strategy/exceptions.py` & `pynonymizer-2.1.1/pynonymizer/strategy/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/strategy/parser.py` & `pynonymizer-2.1.1/pynonymizer/strategy/parser.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/strategy/table.py` & `pynonymizer-2.1.1/pynonymizer/strategy/table.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer/strategy/update_column.py` & `pynonymizer-2.1.1/pynonymizer/strategy/update_column.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/pynonymizer.egg-info/PKG-INFO` & `pynonymizer-2.1.1/pynonymizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynonymizer
-Version: 2.1.0
+Version: 2.1.1
 Summary: An anonymization tool for production databases
 Home-page: https://github.com/rwnx/pynonymizer
 Author: Rowan Twell
 Author-email: rowantwell@gmail.com
 License: MIT
 Keywords: anonymization gdpr database mysql
 Classifier: Development Status :: 5 - Production/Stable
@@ -80,17 +80,14 @@
 1. Restore from dumpfile to temporary database.
 1. Anonymize temporary database with strategy.
 1. Dump resulting data to file.
 1. Drop temporary database.
 
 If this workflow doesnt work for you, see [process control](https://github.com/rwnx/pynonymizer/blob/main/doc/process-control.md) to see if it can be adjusted to suit your needs.
 
-## Requirements
-* Python >= 3.6
-
 ### mysql
 * `mysql`/`mysqldump` Must be in $PATH
 * Local or remote mysql >= 5.5
 * Supported Inputs:
   * Plain SQL over stdout
   * Plain SQL file `.sql`
   * GZip-compressed SQL file `.gz`
```

### Comparing `pynonymizer-2.1.0/pynonymizer.egg-info/SOURCES.txt` & `pynonymizer-2.1.1/pynonymizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.0/setup.py` & `pynonymizer-2.1.1/setup.py`

 * *Files identical despite different names*

