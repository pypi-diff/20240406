# Comparing `tmp/fundamentals-2.6.2.tar.gz` & `tmp/fundamentals-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundamentals-2.6.2.tar", last modified: Fri Jan 19 11:17:46 2024, max compression
+gzip compressed data, was "fundamentals-2.6.3.tar", last modified: Sat Apr  6 21:00:43 2024, max compression
```

## Comparing `fundamentals-2.6.2.tar` & `fundamentals-2.6.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 11:17:46.188384 fundamentals-2.6.2/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      412 2024-01-19 11:08:21.000000 fundamentals-2.6.2/.readthedocs.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4171 2024-01-19 11:08:21.000000 fundamentals-2.6.2/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2024-01-19 11:08:21.000000 fundamentals-2.6.2/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      363 2024-01-19 11:08:21.000000 fundamentals-2.6.2/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3493 2024-01-19 11:17:46.188384 fundamentals-2.6.2/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2548 2024-01-19 11:08:21.000000 fundamentals-2.6.2/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 11:17:46.180384 fundamentals-2.6.2/fundamentals/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      351 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3944 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 11:17:46.180384 fundamentals-2.6.2/fundamentals/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      106 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      375 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/commonutils/getpackagepath.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5696 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/daemonise.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 11:17:46.184384 fundamentals-2.6.2/fundamentals/download/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      477 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/download/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1192 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/download/_dump_files_to_local_drive.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1767 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/download/_fetch.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1564 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/download/append_now_datestamp_to_filename.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1369 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/download/extract_filename_from_url.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      997 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/download/get_now_datetime_filestamp.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6824 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/download/multiobject_download.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 11:17:46.184384 fundamentals-2.6.2/fundamentals/files/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      306 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/files/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1765 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/files/fileChunker.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2121 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2929 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/files/recursive_directory_listing.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6445 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/files/tag.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3087 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/fmultiprocess.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11610 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/logs.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 11:17:46.184384 fundamentals-2.6.2/fundamentals/mysql/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      742 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    21529 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/convert_dictionary_to_mysql_table.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5579 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/database.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13993 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/directory_script_runner.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1584 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/get_database_table_column_names.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13232 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2801 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/readquery.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2460 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/setup_database_connection.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10966 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/sqlite2mysql.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1406 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/table_exists.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7416 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/writequery.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9717 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/mysql/yaml_to_database.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 11:17:46.188384 fundamentals-2.6.2/fundamentals/nose2_plugins/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       41 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/nose2_plugins/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1384 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/nose2_plugins/cprof.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 11:17:46.188384 fundamentals-2.6.2/fundamentals/renderer/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      162 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/renderer/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    20625 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/renderer/list_of_dictionaries.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 11:17:46.188384 fundamentals-2.6.2/fundamentals/stats/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/stats/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2854 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/stats/rolling_window_sigma_clip.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3137 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/times.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23765 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/tools.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5328 2024-01-19 11:08:21.000000 fundamentals-2.6.2/fundamentals/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 11:17:46.180384 fundamentals-2.6.2/fundamentals.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3493 2024-01-19 11:17:46.000000 fundamentals-2.6.2/fundamentals.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1902 2024-01-19 11:17:46.000000 fundamentals-2.6.2/fundamentals.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-01-19 11:17:46.000000 fundamentals-2.6.2/fundamentals.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      183 2024-01-19 11:17:46.000000 fundamentals-2.6.2/fundamentals.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-01-19 11:13:22.000000 fundamentals-2.6.2/fundamentals.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       80 2024-01-19 11:17:46.000000 fundamentals-2.6.2/fundamentals.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       13 2024-01-19 11:17:46.000000 fundamentals-2.6.2/fundamentals.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       79 2024-01-19 11:17:46.188384 fundamentals-2.6.2/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2232 2024-01-19 11:08:21.000000 fundamentals-2.6.2/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-06 21:00:43.567761 fundamentals-2.6.3/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      412 2024-04-06 20:50:48.000000 fundamentals-2.6.3/.readthedocs.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4282 2024-04-06 20:50:48.000000 fundamentals-2.6.3/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2024-04-06 20:50:48.000000 fundamentals-2.6.3/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      363 2024-04-06 20:50:48.000000 fundamentals-2.6.3/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3599 2024-04-06 21:00:43.567761 fundamentals-2.6.3/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2654 2024-04-06 20:50:48.000000 fundamentals-2.6.3/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-06 21:00:43.531759 fundamentals-2.6.3/fundamentals/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      351 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3944 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-06 21:00:43.531759 fundamentals-2.6.3/fundamentals/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      106 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      375 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/commonutils/getpackagepath.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5696 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/daemonise.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-06 21:00:43.535760 fundamentals-2.6.3/fundamentals/download/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      477 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/download/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1192 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/download/_dump_files_to_local_drive.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1767 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/download/_fetch.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1564 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/download/append_now_datestamp_to_filename.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1369 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/download/extract_filename_from_url.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      997 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/download/get_now_datetime_filestamp.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6824 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/download/multiobject_download.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-06 21:00:43.535760 fundamentals-2.6.3/fundamentals/files/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      306 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/files/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1765 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/files/fileChunker.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2121 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2929 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/files/recursive_directory_listing.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6445 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/files/tag.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3087 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/fmultiprocess.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11610 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/logs.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-06 21:00:43.563760 fundamentals-2.6.3/fundamentals/mysql/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      742 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    21529 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/convert_dictionary_to_mysql_table.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5579 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/database.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13993 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/directory_script_runner.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1584 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/get_database_table_column_names.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13281 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2801 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/readquery.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2460 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/setup_database_connection.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10966 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/sqlite2mysql.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1406 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/table_exists.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7416 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/writequery.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9717 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/mysql/yaml_to_database.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-06 21:00:43.563760 fundamentals-2.6.3/fundamentals/nose2_plugins/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       41 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/nose2_plugins/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1384 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/nose2_plugins/cprof.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-06 21:00:43.567761 fundamentals-2.6.3/fundamentals/renderer/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      162 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/renderer/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    20625 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/renderer/list_of_dictionaries.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-06 21:00:43.567761 fundamentals-2.6.3/fundamentals/stats/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/stats/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2854 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/stats/rolling_window_sigma_clip.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3137 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/times.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23765 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/tools.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5328 2024-04-06 20:50:48.000000 fundamentals-2.6.3/fundamentals/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-06 21:00:43.531759 fundamentals-2.6.3/fundamentals.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3599 2024-04-06 21:00:43.000000 fundamentals-2.6.3/fundamentals.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1902 2024-04-06 21:00:43.000000 fundamentals-2.6.3/fundamentals.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-04-06 21:00:43.000000 fundamentals-2.6.3/fundamentals.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      183 2024-04-06 21:00:43.000000 fundamentals-2.6.3/fundamentals.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-04-06 20:55:51.000000 fundamentals-2.6.3/fundamentals.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       80 2024-04-06 21:00:43.000000 fundamentals-2.6.3/fundamentals.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       13 2024-04-06 21:00:43.000000 fundamentals-2.6.3/fundamentals.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       79 2024-04-06 21:00:43.571761 fundamentals-2.6.3/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2232 2024-04-06 20:50:48.000000 fundamentals-2.6.3/setup.py
```

### Comparing `fundamentals-2.6.2/CHANGES.md` & `fundamentals-2.6.3/CHANGES.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 
 ## Release Notes
 
+**v2.6.3 - April 6, 2024**
+
+* **FIXED** fixing 'insert_list_of_dictionaries_into_database_tables' for MySQL 8
+
 **v2.6.2 - January 19, 2024**
 
 * **FIXED** bug fix in collecting settings files from the default location
 
 **v2.6.1 - December 3, 2023**
 
 * **FIXED** fixing logging colours for white terminal backgrounds
```

### Comparing `fundamentals-2.6.2/LICENSE` & `fundamentals-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/PKG-INFO` & `fundamentals-2.6.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fundamentals
-Version: 2.6.2
+Version: 2.6.3
 Summary: Some fundamental tools required by most self-respecting python-packages bundled in one place. Very opinionated project setup tools including logging, plain-text settings files and database connections.
 Home-page: https://github.com/thespacedoctor/fundamentals
-Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.6.2.zip
+Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.6.3.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
 Keywords: logging, database
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -22,17 +22,15 @@
 Requires-Dist: python-dateutil
 Requires-Dist: requests
 Requires-Dist: python-daemon
 
 # fundamentals
 
 
-[![](https://zenodo.org/badge/52598459.svg)](https://zenodo.org/badge/latestdoi/52598459) 
-
-
+[![](https://zenodo.org/badge/DOI/10.5281/zenodo.8037509.svg)](https://zenodo.org/doi/10.5281/zenodo.8037509) 
 
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/fundamentals)](https://pypi.org/project/fundamentals/)
 [![](https://img.shields.io/pypi/v/fundamentals)](https://pypi.org/project/fundamentals/)
 [![](https://img.shields.io/conda/vn/conda-forge/fundamentals.svg)](https://anaconda.org/conda-forge/fundamentals)
 [![](https://pepy.tech/badge/fundamentals)](https://pepy.tech/project/fundamentals)
@@ -57,17 +55,17 @@
 ## How to cite fundamentals
 
 If you use `fundamentals` in your work, please cite using the following BibTeX entry: 
 
 ```bibtex
 @software{Young_fundamentals,
     author = {Young, David R.},
-    doi = {10.5281/zenodo.8037510},
+    doi = {10.5281/zenodo.8037509},
     license = {GPL-3.0-only},
-    title = {{fundamentals}},
-    url = {https://github.com/thespacedoctor/fundamentals}
+    title = {{fundamentals. Fundamental tools required by most self-respecting python-packages bundled in one place}},
+    url = {https://zenodo.org/doi/10.5281/zenodo.8037509}
 }
 ```
```

### Comparing `fundamentals-2.6.2/README.md` & `fundamentals-2.6.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # fundamentals
 
 
-[![](https://zenodo.org/badge/52598459.svg)](https://zenodo.org/badge/latestdoi/52598459) 
-
-
+[![](https://zenodo.org/badge/DOI/10.5281/zenodo.8037509.svg)](https://zenodo.org/doi/10.5281/zenodo.8037509) 
 
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/fundamentals)](https://pypi.org/project/fundamentals/)
 [![](https://img.shields.io/pypi/v/fundamentals)](https://pypi.org/project/fundamentals/)
 [![](https://img.shields.io/conda/vn/conda-forge/fundamentals.svg)](https://anaconda.org/conda-forge/fundamentals)
 [![](https://pepy.tech/badge/fundamentals)](https://pepy.tech/project/fundamentals)
@@ -32,17 +30,17 @@
 ## How to cite fundamentals
 
 If you use `fundamentals` in your work, please cite using the following BibTeX entry: 
 
 ```bibtex
 @software{Young_fundamentals,
     author = {Young, David R.},
-    doi = {10.5281/zenodo.8037510},
+    doi = {10.5281/zenodo.8037509},
     license = {GPL-3.0-only},
-    title = {{fundamentals}},
-    url = {https://github.com/thespacedoctor/fundamentals}
+    title = {{fundamentals. Fundamental tools required by most self-respecting python-packages bundled in one place}},
+    url = {https://zenodo.org/doi/10.5281/zenodo.8037509}
 }
 ```
```

### Comparing `fundamentals-2.6.2/fundamentals/cl_utils.py` & `fundamentals-2.6.3/fundamentals/cl_utils.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/daemonise.py` & `fundamentals-2.6.3/fundamentals/daemonise.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/download/_dump_files_to_local_drive.py` & `fundamentals-2.6.3/fundamentals/download/_dump_files_to_local_drive.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/download/_fetch.py` & `fundamentals-2.6.3/fundamentals/download/_fetch.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/download/append_now_datestamp_to_filename.py` & `fundamentals-2.6.3/fundamentals/download/append_now_datestamp_to_filename.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/download/extract_filename_from_url.py` & `fundamentals-2.6.3/fundamentals/download/extract_filename_from_url.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/download/get_now_datetime_filestamp.py` & `fundamentals-2.6.3/fundamentals/download/get_now_datetime_filestamp.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/download/multiobject_download.py` & `fundamentals-2.6.3/fundamentals/download/multiobject_download.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/files/fileChunker.py` & `fundamentals-2.6.3/fundamentals/files/fileChunker.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py` & `fundamentals-2.6.3/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/files/recursive_directory_listing.py` & `fundamentals-2.6.3/fundamentals/files/recursive_directory_listing.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/files/tag.py` & `fundamentals-2.6.3/fundamentals/files/tag.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/fmultiprocess.py` & `fundamentals-2.6.3/fundamentals/fmultiprocess.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/logs.py` & `fundamentals-2.6.3/fundamentals/logs.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/__init__.py` & `fundamentals-2.6.3/fundamentals/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/convert_dictionary_to_mysql_table.py` & `fundamentals-2.6.3/fundamentals/mysql/convert_dictionary_to_mysql_table.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/database.py` & `fundamentals-2.6.3/fundamentals/mysql/database.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/directory_script_runner.py` & `fundamentals-2.6.3/fundamentals/mysql/directory_script_runner.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/get_database_table_column_names.py` & `fundamentals-2.6.3/fundamentals/mysql/get_database_table_column_names.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py` & `fundamentals-2.6.3/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,16 +404,17 @@
         log=log,
         sqlQuery=sqlQuery,
         dbConn=dbConn
     )
 
     csvColumns = [k for d in dictList for k in list(d.keys())]
     csvColumns = list(set(csvColumns))
-    csvColumnsString = (', ').join(csvColumns)
-    csvColumnsString = csvColumnsString.replace(u" dec,", u" decl,")
+    csvColumnsString = ('`, `').join(csvColumns)
+    csvColumnsString = f'`{csvColumnsString}`'
+    csvColumnsString = csvColumnsString.replace(u'`dec`', u'`decl`')
 
     df = pd.DataFrame(dictList)
     df.replace(['nan', 'None', '', 'NaN', np.nan], '\\N', inplace=True)
     df.to_csv('/tmp/%(tmpTable)s' % locals(), sep="|",
               index=False, escapechar="\\", quotechar='"', columns=csvColumns, encoding='utf-8')
 
     sqlQuery = """LOAD DATA LOCAL INFILE '/tmp/%(tmpTable)s'
```

### Comparing `fundamentals-2.6.2/fundamentals/mysql/readquery.py` & `fundamentals-2.6.3/fundamentals/mysql/readquery.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/setup_database_connection.py` & `fundamentals-2.6.3/fundamentals/mysql/setup_database_connection.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/sqlite2mysql.py` & `fundamentals-2.6.3/fundamentals/mysql/sqlite2mysql.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/table_exists.py` & `fundamentals-2.6.3/fundamentals/mysql/table_exists.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/writequery.py` & `fundamentals-2.6.3/fundamentals/mysql/writequery.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/mysql/yaml_to_database.py` & `fundamentals-2.6.3/fundamentals/mysql/yaml_to_database.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/nose2_plugins/cprof.py` & `fundamentals-2.6.3/fundamentals/nose2_plugins/cprof.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/renderer/list_of_dictionaries.py` & `fundamentals-2.6.3/fundamentals/renderer/list_of_dictionaries.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/stats/rolling_window_sigma_clip.py` & `fundamentals-2.6.3/fundamentals/stats/rolling_window_sigma_clip.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/times.py` & `fundamentals-2.6.3/fundamentals/times.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/tools.py` & `fundamentals-2.6.3/fundamentals/tools.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals/utKit.py` & `fundamentals-2.6.3/fundamentals/utKit.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/fundamentals.egg-info/PKG-INFO` & `fundamentals-2.6.3/fundamentals.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fundamentals
-Version: 2.6.2
+Version: 2.6.3
 Summary: Some fundamental tools required by most self-respecting python-packages bundled in one place. Very opinionated project setup tools including logging, plain-text settings files and database connections.
 Home-page: https://github.com/thespacedoctor/fundamentals
-Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.6.2.zip
+Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.6.3.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
 Keywords: logging, database
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -22,17 +22,15 @@
 Requires-Dist: python-dateutil
 Requires-Dist: requests
 Requires-Dist: python-daemon
 
 # fundamentals
 
 
-[![](https://zenodo.org/badge/52598459.svg)](https://zenodo.org/badge/latestdoi/52598459) 
-
-
+[![](https://zenodo.org/badge/DOI/10.5281/zenodo.8037509.svg)](https://zenodo.org/doi/10.5281/zenodo.8037509) 
 
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/fundamentals)](https://pypi.org/project/fundamentals/)
 [![](https://img.shields.io/pypi/v/fundamentals)](https://pypi.org/project/fundamentals/)
 [![](https://img.shields.io/conda/vn/conda-forge/fundamentals.svg)](https://anaconda.org/conda-forge/fundamentals)
 [![](https://pepy.tech/badge/fundamentals)](https://pepy.tech/project/fundamentals)
@@ -57,17 +55,17 @@
 ## How to cite fundamentals
 
 If you use `fundamentals` in your work, please cite using the following BibTeX entry: 
 
 ```bibtex
 @software{Young_fundamentals,
     author = {Young, David R.},
-    doi = {10.5281/zenodo.8037510},
+    doi = {10.5281/zenodo.8037509},
     license = {GPL-3.0-only},
-    title = {{fundamentals}},
-    url = {https://github.com/thespacedoctor/fundamentals}
+    title = {{fundamentals. Fundamental tools required by most self-respecting python-packages bundled in one place}},
+    url = {https://zenodo.org/doi/10.5281/zenodo.8037509}
 }
 ```
```

### Comparing `fundamentals-2.6.2/fundamentals.egg-info/SOURCES.txt` & `fundamentals-2.6.3/fundamentals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.2/setup.py` & `fundamentals-2.6.3/setup.py`

 * *Files identical despite different names*

