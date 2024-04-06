# Comparing `tmp/tulona-0.2.1.tar.gz` & `tmp/tulona-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.2.1.tar", last modified: Fri Apr  5 04:16:51 2024, max compression
+gzip compressed data, was "tulona-0.2.2.tar", last modified: Sat Apr  6 09:09:56 2024, max compression
```

## Comparing `tulona-0.2.1.tar` & `tulona-0.2.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.600195 tulona-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-05 04:16:47.000000 tulona-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-05 04:16:51.600195 tulona-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-05 04:16:47.000000 tulona-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.592195 tulona-0.2.1/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.592195 tulona-0.2.1/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.592195 tulona-0.2.1/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.592195 tulona-0.2.1/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.596195 tulona-0.2.1/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.596195 tulona-0.2.1/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.596195 tulona-0.2.1/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/task/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/task/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.596195 tulona-0.2.1/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.596195 tulona-0.2.1/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-05 04:16:47.000000 tulona-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:16:51.600195 tulona-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:56.233359 tulona-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-06 09:09:47.000000 tulona-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-06 09:09:56.233359 tulona-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-06 09:09:47.000000 tulona-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:56.225360 tulona-0.2.2/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:56.225360 tulona-0.2.2/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:56.229359 tulona-0.2.2/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:56.229359 tulona-0.2.2/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:56.229359 tulona-0.2.2/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:56.229359 tulona-0.2.2/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:56.229359 tulona-0.2.2/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/task/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/task/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:56.233359 tulona-0.2.2/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/util/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-06 09:09:47.000000 tulona-0.2.2/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:09:56.233359 tulona-0.2.2/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-06 09:09:56.000000 tulona-0.2.2/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 09:09:56.000000 tulona-0.2.2/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:09:56.000000 tulona-0.2.2/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-06 09:09:56.000000 tulona-0.2.2/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-06 09:09:56.000000 tulona-0.2.2/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 09:09:56.000000 tulona-0.2.2/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-06 09:09:47.000000 tulona-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 09:09:56.233359 tulona-0.2.2/setup.cfg
```

### Comparing `tulona-0.2.1/LICENSE` & `tulona-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/adapter/connection.py` & `tulona-0.2.2/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/adapter/mssql.py` & `tulona-0.2.2/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/adapter/mysql.py` & `tulona-0.2.2/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/adapter/postgres.py` & `tulona-0.2.2/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/adapter/snowflake.py` & `tulona-0.2.2/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/cli/base.py` & `tulona-0.2.2/core/tulona/cli/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,16 @@
 def compare_column(ctx, **kwargs):
     """
     Column name must be specified for task: compare-column
     either by specifying 'compare_column' property in
     at least one of the datasource[project] configs
     (check sample tulona-project.yml file for example)
     or with '--datasources' command line argument
-    using one of the following formats (column name is same for option 3 and 4):-
+    using one of the following formats
+    (column name is same for option 3 and 4):-
     1. <datasource1>:<col1>,<datasource2>:<col2>
     2. <datasource1>:<col>,<datasource2>:<col>
     3. <datasource1>:<col>,<datasource2>
     4. <datasource1>,<datasource2>:<col>
     """
 
     if "datasources" not in kwargs:
```

### Comparing `tulona-0.2.1/core/tulona/cli/params.py` & `tulona-0.2.2/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/config/profile.py` & `tulona-0.2.2/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/config/project.py` & `tulona-0.2.2/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/exceptions.py` & `tulona-0.2.2/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/task/base.py` & `tulona-0.2.2/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/task/compare.py` & `tulona-0.2.2/core/tulona/task/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,17 +163,17 @@
         else:
             raise TulonaMissingPrimaryKeyError(
                 "Primary key is required for data comparison"
             )
 
         # Exclude columns
         log.debug("Excluding columns")
-        if 'exclude_columns' in ds_dict1:
+        if "exclude_columns" in ds_dict1:
             df1 = apply_column_exclusion(df1, ds_dict1, table_name1)
-        if 'exclude_columns' in ds_dict2:
+        if "exclude_columns" in ds_dict2:
             df2 = apply_column_exclusion(df2, ds_dict2, table_name2)
 
         # Compare
         common_columns = list(
             set(df1.columns)
             .intersection(set(df2.columns))
             .union({ds_dict1["primary_key"].lower()})
@@ -278,15 +278,16 @@
         else:
             raise TulonaMissingPropertyError(
                 "Column name must be specified for task: compare-column"
                 " either by specifying 'compare_column' property in"
                 " at least one of the datasource[project] configs"
                 " (check sample tulona-project.yml file for example)"
                 " or with '--datasources' command line argument"
-                " using one of the following formats (column name is same for option 3 and 4):-"
+                " using one of the following formats"
+                " (column name is same for option 3 and 4):-"
                 " 1. <datasource1>:<col1>,<datasource2>:<col2>"
                 " 2. <datasource1>:<col>,<datasource2>:<col>"
                 " 3. <datasource1>:<col>,<datasource2>"
                 " 4. <datasource1>,<datasource2>:<col>"
             )
 
         ds_dict1 = self.project["datasources"][datasource1]
```

### Comparing `tulona-0.2.1/core/tulona/task/profile.py` & `tulona-0.2.2/core/tulona/task/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/task/scan.py` & `tulona-0.2.2/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/task/test_connection.py` & `tulona-0.2.2/core/tulona/task/test_connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/util/database.py` & `tulona-0.2.2/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/util/dataframe.py` & `tulona-0.2.2/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/util/excel.py` & `tulona-0.2.2/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/util/filesystem.py` & `tulona-0.2.2/core/tulona/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/util/profiles.py` & `tulona-0.2.2/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona/util/sql.py` & `tulona-0.2.2/core/tulona/util/sql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/core/tulona.egg-info/SOURCES.txt` & `tulona-0.2.2/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.2.1/pyproject.toml` & `tulona-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.2.1"
+version = "0.2.2"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -24,14 +24,15 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 keywords = [
   "tulona",
   "comparison",
   "data comparison",
   "database scan",
   "database profile",
@@ -92,8 +93,31 @@
   "raise TulonaMissingPrimaryKeyError",
   "raise TulonaFundamentalError",
 ]
 
 [tool.isort]
 profile = "black"
 line_length = 90
-skip = [".gitignore"]
+skip = [".gitignore"]
+
+[tool.bumpversion]
+current_version = "0.2.2"
+parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
+serialize = ["{major}.{minor}.{patch}"]
+search = "{current_version}"
+replace = "{new_version}"
+regex = false
+ignore_missing_version = false
+tag = false
+sign_tags = false
+tag_name = "v{new_version}"
+tag_message = "Bump version: {current_version} → {new_version}"
+allow_dirty = false
+commit = true
+message = "Bump version: {current_version} → {new_version}"
+commit_args = ""
+
+[[tool.bumpversion.files]]
+filename = "pyproject.toml"
+
+[[tool.bumpversion.files]]
+filename = "core/setup.py"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

