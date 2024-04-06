# Comparing `tmp/lapa_database_structure-0.0.6.tar.gz` & `tmp/lapa_database_structure-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapa_database_structure-0.0.6.tar", last modified: Fri Mar  8 09:43:09 2024, max compression
+gzip compressed data, was "lapa_database_structure-0.0.7.tar", last modified: Sat Apr  6 15:08:10 2024, max compression
```

## Comparing `lapa_database_structure-0.0.6.tar` & `lapa_database_structure-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.541335 lapa_database_structure-0.0.6/lapa_database_structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/lapa_database_structure/lapa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/lapa_database_structure/lapa/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa/authentication/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/lapa_database_structure/lapa/file_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa/file_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa/file_storage/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/lapa_database_structure/lapa/public/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa/public/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/authentication/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/file_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/file_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/file_storage/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/public/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/public/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/lapa_database_structure/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:43:09.541335 lapa_database_structure-0.0.6/lapa_database_structure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-08 09:43:09.000000 lapa_database_structure-0.0.6/lapa_database_structure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-08 09:43:09.000000 lapa_database_structure-0.0.6/lapa_database_structure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 09:43:09.000000 lapa_database_structure-0.0.6/lapa_database_structure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-08 09:43:09.000000 lapa_database_structure-0.0.6/lapa_database_structure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-08 09:43:09.000000 lapa_database_structure-0.0.6/lapa_database_structure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 09:43:09.545335 lapa_database_structure-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-08 09:43:00.000000 lapa_database_structure-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.441500 lapa_database_structure-0.0.7/lapa_database_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.441500 lapa_database_structure-0.0.7/lapa_database_structure/lapa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/authentication/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa/file_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/file_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/file_storage/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa/public/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/public/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/authentication/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/file_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/file_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/file_storage/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/public/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/public/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.441500 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-06 15:08:10.000000 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-06 15:08:10.000000 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:08:10.000000 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 15:08:10.000000 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 15:08:10.000000 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/setup.py
```

### Comparing `lapa_database_structure-0.0.6/PKG-INFO` & `lapa_database_structure-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapa_database_structure
-Version: 0.0.6
+Version: 0.0.7
 Summary: database layer for my personal server.
 Home-page: https://github.com/B21amish/lapa_database_structure
 Author: Amish Palkar, thePmSquare, Lav Sharma,Aaditya Sangishetty
 Author-email: amishpalkar302001@gmail.com, thepmsquare@gmail.com, lavsharma2016@gmail.com, adityasehtty35@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -55,14 +55,19 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.7
+
+-  Overhauled authentication schema, 
+- introducing new tables: User, UsernameAuthentication, UserProfile, AuthenticationType, UserAccountStatus, UserLog, and UserLogStatus.
+
 ### v0.0.6
 
 - changed db structure
 - removed game db
 - added testing db which is clone of lapa
 
 ### v0.0.5
```

### Comparing `lapa_database_structure-0.0.6/README.md` & `lapa_database_structure-0.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.7
+
+-  Overhauled authentication schema, 
+- introducing new tables: User, UsernameAuthentication, UserProfile, AuthenticationType, UserAccountStatus, UserLog, and UserLogStatus.
+
 ### v0.0.6
 
 - changed db structure
 - removed game db
 - added testing db which is clone of lapa
 
 ### v0.0.5
```

### Comparing `lapa_database_structure-0.0.6/lapa_database_structure/lapa/file_storage/tables.py` & `lapa_database_structure-0.0.7/lapa_database_structure/lapa/file_storage/tables.py`

 * *Files identical despite different names*

### Comparing `lapa_database_structure-0.0.6/lapa_database_structure/lapa_testing/file_storage/tables.py` & `lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/file_storage/tables.py`

 * *Files identical despite different names*

### Comparing `lapa_database_structure-0.0.6/lapa_database_structure.egg-info/PKG-INFO` & `lapa_database_structure-0.0.7/lapa_database_structure.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapa-database-structure
-Version: 0.0.6
+Version: 0.0.7
 Summary: database layer for my personal server.
 Home-page: https://github.com/B21amish/lapa_database_structure
 Author: Amish Palkar, thePmSquare, Lav Sharma,Aaditya Sangishetty
 Author-email: amishpalkar302001@gmail.com, thepmsquare@gmail.com, lavsharma2016@gmail.com, adityasehtty35@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -55,14 +55,19 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.7
+
+-  Overhauled authentication schema, 
+- introducing new tables: User, UsernameAuthentication, UserProfile, AuthenticationType, UserAccountStatus, UserLog, and UserLogStatus.
+
 ### v0.0.6
 
 - changed db structure
 - removed game db
 - added testing db which is clone of lapa
 
 ### v0.0.5
```

### Comparing `lapa_database_structure-0.0.6/lapa_database_structure.egg-info/SOURCES.txt` & `lapa_database_structure-0.0.7/lapa_database_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lapa_database_structure-0.0.6/setup.py` & `lapa_database_structure-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 package_name = "lapa_database_structure"
 
 setup(
     name=package_name,
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(),
     package_data={
         package_name: [],
     },
     install_requires=[
         "sqlalchemy>=2.0.23",
     ],
```

