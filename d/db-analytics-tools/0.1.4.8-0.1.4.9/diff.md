# Comparing `tmp/db_analytics_tools-0.1.4.8.tar.gz` & `tmp/db_analytics_tools-0.1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_analytics_tools-0.1.4.8.tar", last modified: Sat Sep 16 18:36:51 2023, max compression
+gzip compressed data, was "db_analytics_tools-0.1.4.9.tar", last modified: Sun Sep 17 14:27:31 2023, max compression
```

## Comparing `db_analytics_tools-0.1.4.8.tar` & `db_analytics_tools-0.1.4.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 18:36:51.438341 db_analytics_tools-0.1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-16 18:36:42.000000 db_analytics_tools-0.1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2023-09-16 18:36:51.434341 db_analytics_tools-0.1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10046 2023-09-16 18:36:42.000000 db_analytics_tools-0.1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 18:36:51.434341 db_analytics_tools-0.1.4.8/db_analytics_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-09-16 18:36:42.000000 db_analytics_tools-0.1.4.8/db_analytics_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-16 18:36:42.000000 db_analytics_tools-0.1.4.8/db_analytics_tools/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2023-09-16 18:36:42.000000 db_analytics_tools-0.1.4.8/db_analytics_tools/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-16 18:36:42.000000 db_analytics_tools-0.1.4.8/db_analytics_tools/learning.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-09-16 18:36:42.000000 db_analytics_tools-0.1.4.8/db_analytics_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-09-16 18:36:42.000000 db_analytics_tools-0.1.4.8/db_analytics_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 18:36:51.434341 db_analytics_tools-0.1.4.8/db_analytics_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2023-09-16 18:36:51.000000 db_analytics_tools-0.1.4.8/db_analytics_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-09-16 18:36:51.000000 db_analytics_tools-0.1.4.8/db_analytics_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-16 18:36:51.000000 db_analytics_tools-0.1.4.8/db_analytics_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-09-16 18:36:51.000000 db_analytics_tools-0.1.4.8/db_analytics_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-16 18:36:51.000000 db_analytics_tools-0.1.4.8/db_analytics_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-16 18:36:51.438341 db_analytics_tools-0.1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-09-16 18:36:42.000000 db_analytics_tools-0.1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 14:27:31.761855 db_analytics_tools-0.1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-17 14:27:20.000000 db_analytics_tools-0.1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2023-09-17 14:27:31.761855 db_analytics_tools-0.1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2023-09-17 14:27:20.000000 db_analytics_tools-0.1.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 14:27:31.761855 db_analytics_tools-0.1.4.9/db_analytics_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2023-09-17 14:27:20.000000 db_analytics_tools-0.1.4.9/db_analytics_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-17 14:27:20.000000 db_analytics_tools-0.1.4.9/db_analytics_tools/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2023-09-17 14:27:20.000000 db_analytics_tools-0.1.4.9/db_analytics_tools/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-17 14:27:20.000000 db_analytics_tools-0.1.4.9/db_analytics_tools/learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2023-09-17 14:27:20.000000 db_analytics_tools-0.1.4.9/db_analytics_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2023-09-17 14:27:20.000000 db_analytics_tools-0.1.4.9/db_analytics_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 14:27:31.761855 db_analytics_tools-0.1.4.9/db_analytics_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2023-09-17 14:27:31.000000 db_analytics_tools-0.1.4.9/db_analytics_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2023-09-17 14:27:31.000000 db_analytics_tools-0.1.4.9/db_analytics_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-17 14:27:31.000000 db_analytics_tools-0.1.4.9/db_analytics_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-09-17 14:27:31.000000 db_analytics_tools-0.1.4.9/db_analytics_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-17 14:27:31.000000 db_analytics_tools-0.1.4.9/db_analytics_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-17 14:27:31.761855 db_analytics_tools-0.1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-09-17 14:27:20.000000 db_analytics_tools-0.1.4.9/setup.py
```

### Comparing `db_analytics_tools-0.1.4.8/LICENSE` & `db_analytics_tools-0.1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `db_analytics_tools-0.1.4.8/PKG-INFO` & `db_analytics_tools-0.1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db_analytics_tools
-Version: 0.1.4.8
+Version: 0.1.4.9
 Summary: Databases Tools for Data Analytics
 Home-page: https://josephkonka.com/#projects
 Download-URL: https://github.com/joekakone/db-analytics-tools
 Author: Joseph Konka
 Author-email: contact@josephkonka.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/joekakone/db-analytics-tools/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: db_analytics_tools Version: 0.1.4.8 Summary:
+Metadata-Version: 2.1 Name: db_analytics_tools Version: 0.1.4.9 Summary:
 Databases Tools for Data Analytics Home-page: https://josephkonka.com/#projects
 Download-URL: https://github.com/joekakone/db-analytics-tools Author: Joseph
 Konka Author-email: contact@josephkonka.com License: MIT Project-URL: Bug
 Tracker, https://github.com/joekakone/db-analytics-tools/issues Project-URL:
 Documentation, https://joekakone.github.io/db-analytics-tools Project-URL:
 Source Code, https://github.com/joekakone/db-analytics-tools Keywords:
 databases analytics etl sql orc Requires-Python: >=3.6 Description-Content-
```

### Comparing `db_analytics_tools-0.1.4.8/README.md` & `db_analytics_tools-0.1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `db_analytics_tools-0.1.4.8/db_analytics_tools.egg-info/PKG-INFO` & `db_analytics_tools-0.1.4.9/db_analytics_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-analytics-tools
-Version: 0.1.4.8
+Version: 0.1.4.9
 Summary: Databases Tools for Data Analytics
 Home-page: https://josephkonka.com/#projects
 Download-URL: https://github.com/joekakone/db-analytics-tools
 Author: Joseph Konka
 Author-email: contact@josephkonka.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/joekakone/db-analytics-tools/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: db-analytics-tools Version: 0.1.4.8 Summary:
+Metadata-Version: 2.1 Name: db-analytics-tools Version: 0.1.4.9 Summary:
 Databases Tools for Data Analytics Home-page: https://josephkonka.com/#projects
 Download-URL: https://github.com/joekakone/db-analytics-tools Author: Joseph
 Konka Author-email: contact@josephkonka.com License: MIT Project-URL: Bug
 Tracker, https://github.com/joekakone/db-analytics-tools/issues Project-URL:
 Documentation, https://joekakone.github.io/db-analytics-tools Project-URL:
 Source Code, https://github.com/joekakone/db-analytics-tools Keywords:
 databases analytics etl sql orc Requires-Python: >=3.6 Description-Content-
```

### Comparing `db_analytics_tools-0.1.4.8/setup.py` & `db_analytics_tools-0.1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="db_analytics_tools",
-    version="0.1.4.8",
+    version="0.1.4.9",
     url="https://josephkonka.com/#projects",
     download_url="https://github.com/joekakone/db-analytics-tools",
     project_urls={
         "Bug Tracker": "https://github.com/joekakone/db-analytics-tools/issues",
         "Documentation": "https://joekakone.github.io/db-analytics-tools",
         "Source Code": "https://github.com/joekakone/db-analytics-tools",
     },
```

