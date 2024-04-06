# Comparing `tmp/zonefile_parser-0.1.8.tar.gz` & `tmp/zonefile_parser-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zonefile_parser-0.1.8.tar", last modified: Sat Apr 17 09:17:20 2021, max compression
+gzip compressed data, was "zonefile_parser-0.1.9.tar", last modified: Mon Apr 19 09:25:39 2021, max compression
```

## Comparing `zonefile_parser-0.1.8.tar` & `zonefile_parser-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 09:17:20.466263 zonefile_parser-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)      837 2021-04-17 09:17:20.466263 zonefile_parser-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-04-17 09:17:08.000000 zonefile_parser-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-04-17 09:17:20.466263 zonefile_parser-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2021-04-17 09:17:08.000000 zonefile_parser-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 09:17:20.466263 zonefile_parser-0.1.8/zonefile_parser/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-17 09:17:08.000000 zonefile_parser-0.1.8/zonefile_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2021-04-17 09:17:08.000000 zonefile_parser-0.1.8/zonefile_parser/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2021-04-17 09:17:08.000000 zonefile_parser-0.1.8/zonefile_parser/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2021-04-17 09:17:08.000000 zonefile_parser-0.1.8/zonefile_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2021-04-17 09:17:08.000000 zonefile_parser-0.1.8/zonefile_parser/record.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 09:17:20.466263 zonefile_parser-0.1.8/zonefile_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      837 2021-04-17 09:17:20.000000 zonefile_parser-0.1.8/zonefile_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-04-17 09:17:20.000000 zonefile_parser-0.1.8/zonefile_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-17 09:17:20.000000 zonefile_parser-0.1.8/zonefile_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-17 09:17:20.000000 zonefile_parser-0.1.8/zonefile_parser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-04-17 09:17:20.000000 zonefile_parser-0.1.8/zonefile_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-19 09:25:39.166994 zonefile_parser-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2021-04-19 09:25:39.166994 zonefile_parser-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-04-19 09:25:29.000000 zonefile_parser-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-04-19 09:25:39.166994 zonefile_parser-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2021-04-19 09:25:29.000000 zonefile_parser-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-19 09:25:39.162994 zonefile_parser-0.1.9/zonefile_parser/
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-19 09:25:29.000000 zonefile_parser-0.1.9/zonefile_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2426 2021-04-19 09:25:29.000000 zonefile_parser-0.1.9/zonefile_parser/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3107 2021-04-19 09:25:29.000000 zonefile_parser-0.1.9/zonefile_parser/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2021-04-19 09:25:29.000000 zonefile_parser-0.1.9/zonefile_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2021-04-19 09:25:29.000000 zonefile_parser-0.1.9/zonefile_parser/record.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-19 09:25:39.166994 zonefile_parser-0.1.9/zonefile_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2021-04-19 09:25:38.000000 zonefile_parser-0.1.9/zonefile_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-04-19 09:25:38.000000 zonefile_parser-0.1.9/zonefile_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-19 09:25:38.000000 zonefile_parser-0.1.9/zonefile_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-19 09:25:38.000000 zonefile_parser-0.1.9/zonefile_parser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-04-19 09:25:38.000000 zonefile_parser-0.1.9/zonefile_parser.egg-info/top_level.txt
```

### Comparing `zonefile_parser-0.1.8/PKG-INFO` & `zonefile_parser-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 1.2
 Name: zonefile_parser
-Version: 0.1.8
+Version: 0.1.9
 Summary: library for parsing dns zone files
 Home-page: https://github.com/aredwood/zone-file-parser
 Author: Alex Redwood
 Author-email: hello@alexredwood.com
 Maintainer: Alex Redwood
 Maintainer-email: hello@alexredwood.com
 License: MIT
-Download-URL: https://github.com/aredwood/zone-file-parser/archive/0.1.8.tar.gz
+Download-URL: https://github.com/aredwood/zone-file-parser/archive/0.1.9.tar.gz
 Description: UNKNOWN
 Keywords: parse dns zone file
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zonefile_parser-0.1.8/README.md` & `zonefile_parser-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `zonefile_parser-0.1.8/setup.py` & `zonefile_parser-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ==============
 
 """
 
 from setuptools import setup, find_packages
 
 
-version = "0.1.8"
+version = "0.1.9"
 
 
 setup(
     name='zonefile_parser',
     version=version,
     url='https://github.com/aredwood/zone-file-parser',
     license='MIT',
```

### Comparing `zonefile_parser-0.1.8/zonefile_parser/helper.py` & `zonefile_parser-0.1.9/zonefile_parser/helper.py`

 * *Files identical despite different names*

### Comparing `zonefile_parser-0.1.8/zonefile_parser/main.py` & `zonefile_parser-0.1.9/zonefile_parser/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,28 +87,24 @@
             lambda x : shlex.split(x),
             normalized_records
         )
     )
 
     # add a TTL to records where one doesn't exist
     def add_ttl(record:list):
-        if record[1] == "IN":
+        if not record[1].isdigit():
             record.insert(1,ttl)
 
         return record
 
     # add an rclass (defaults to IN) when one isn't present
     def add_rclass(record:list):
-        # there are at least 5 required fields for each record
-        if len(record) < 5 and record[1].isdigit():
+        if not (record[2] in ('IN','CS','CH','HS')):
             record.insert(2,default_rclass)
 
-        if len(record) < 5 and record[2].isdigit():
-            record.insert(1,default_rclass)
-
         return record
 
 
     normalized_records = list(
         map(
             lambda x : add_ttl(x),
             normalized_records
```

### Comparing `zonefile_parser-0.1.8/zonefile_parser/parser.py` & `zonefile_parser-0.1.9/zonefile_parser/parser.py`

 * *Files identical despite different names*

### Comparing `zonefile_parser-0.1.8/zonefile_parser/record.py` & `zonefile_parser-0.1.9/zonefile_parser/record.py`

 * *Files identical despite different names*

### Comparing `zonefile_parser-0.1.8/zonefile_parser.egg-info/PKG-INFO` & `zonefile_parser-0.1.9/zonefile_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 1.2
 Name: zonefile-parser
-Version: 0.1.8
+Version: 0.1.9
 Summary: library for parsing dns zone files
 Home-page: https://github.com/aredwood/zone-file-parser
 Author: Alex Redwood
 Author-email: hello@alexredwood.com
 Maintainer: Alex Redwood
 Maintainer-email: hello@alexredwood.com
 License: MIT
-Download-URL: https://github.com/aredwood/zone-file-parser/archive/0.1.8.tar.gz
+Download-URL: https://github.com/aredwood/zone-file-parser/archive/0.1.9.tar.gz
 Description: UNKNOWN
 Keywords: parse dns zone file
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

