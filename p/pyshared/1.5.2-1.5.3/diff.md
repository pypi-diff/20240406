# Comparing `tmp/pyshared-1.5.2-py3-none-any.whl.zip` & `tmp/pyshared-1.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11304 bytes, number of entries: 15
+Zip file size: 11345 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      755 b- defN 24-Apr-04 12:51 pyshared/__init__.py
 -rw-r--r--  2.0 unx      124 b- defN 24-Jan-11 01:53 pyshared/consts.py
 -rw-r--r--  2.0 unx     1293 b- defN 24-Jan-12 03:28 pyshared/crypto.py
 -rw-r--r--  2.0 unx     2029 b- defN 24-Apr-03 16:31 pyshared/env.py
 -rw-r--r--  2.0 unx      943 b- defN 24-Mar-31 21:02 pyshared/exceptions.py
 -rw-r--r--  2.0 unx      914 b- defN 24-Mar-31 21:30 pyshared/pytest.py
 -rw-r--r--  2.0 unx     4929 b- defN 24-Apr-03 16:29 pyshared/python.py
 -rw-r--r--  2.0 unx      790 b- defN 24-Jan-11 05:57 pyshared/shell.py
 -rw-r--r--  2.0 unx     2083 b- defN 24-Jan-12 03:45 pyshared/terminal.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-04 12:52 pyshared/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-04 12:54 pyshared-1.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     6666 b- defN 24-Apr-04 12:54 pyshared-1.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 12:54 pyshared-1.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-04 12:54 pyshared-1.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1138 b- defN 24-Apr-04 12:54 pyshared-1.5.2.dist-info/RECORD
-15 files, 22855 bytes uncompressed, 9444 bytes compressed:  58.7%
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-05 23:00 pyshared/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-05 23:01 pyshared-1.5.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6742 b- defN 24-Apr-05 23:01 pyshared-1.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 23:01 pyshared-1.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-05 23:01 pyshared-1.5.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1138 b- defN 24-Apr-05 23:01 pyshared-1.5.3.dist-info/RECORD
+15 files, 22931 bytes uncompressed, 9485 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pyshared/terminal.py
 Comment: 
 
 Filename: pyshared/version.py
 Comment: 
 
-Filename: pyshared-1.5.2.dist-info/LICENSE
+Filename: pyshared-1.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: pyshared-1.5.2.dist-info/METADATA
+Filename: pyshared-1.5.3.dist-info/METADATA
 Comment: 
 
-Filename: pyshared-1.5.2.dist-info/WHEEL
+Filename: pyshared-1.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyshared-1.5.2.dist-info/top_level.txt
+Filename: pyshared-1.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyshared-1.5.2.dist-info/RECORD
+Filename: pyshared-1.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyshared/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.5.2'
+__version__ = '1.5.3'
```

## Comparing `pyshared-1.5.2.dist-info/LICENSE` & `pyshared-1.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyshared-1.5.2.dist-info/METADATA` & `pyshared-1.5.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshared
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Python library containing common utility functions for use across multiple codebases, filling gaps not covered by the standard Python libraries.
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Cary Carter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,14 +61,16 @@
 Requires-Dist: twine ; extra == 'dev'
 Requires-Dist: build ; extra == 'dev'
 
 # PyShared
 
 PyShared is a Python utility library providing a collection of functions and constants I've found useful across multiple projects.
 
+It also has several common aliases I use for typehints and common imports.
+
 ## Installation
 
 To incorporate PyShared into your project, use pip for installation:
 
 ```bash
 pip install pyshared
 # To include development dependencies:
```

## Comparing `pyshared-1.5.2.dist-info/RECORD` & `pyshared-1.5.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 pyshared/crypto.py,sha256=Ww3uT2xa7g0ewgZzvJthJQ_BRPeHM0sLZPc5c3tad2E,1293
 pyshared/env.py,sha256=sJM9SVUIKVq9n7ugpC81zRhvAlNPur_Q8qUiCasglXQ,2029
 pyshared/exceptions.py,sha256=j7alpB6QyzZcCt9quCWPIKXmSsUw7dZPvs7fdqbYbO4,943
 pyshared/pytest.py,sha256=Sr62vEHhsVtdD6g5oUtpvW07ciYkVhjnCmMCSK_LLnA,914
 pyshared/python.py,sha256=2AsqfdwMGv-ZwXvlaKvaPKmXwq69yFSwKIzQfMblD_E,4929
 pyshared/shell.py,sha256=F2EJdaImnnlxeiONPlzdXcE_JZ1HUAdBWR5_i-WLfSA,790
 pyshared/terminal.py,sha256=6BjoRuUoqU7iKuXhEqU091aOiQWJUcVWXTMeUlNE3MA,2083
-pyshared/version.py,sha256=l_m-0-0bfRsAKcenvAk4AZVqaiD1LKz6_9X_QfaXbtw,22
-pyshared-1.5.2.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
-pyshared-1.5.2.dist-info/METADATA,sha256=kn7nzc-Z1mkTy78Gvudr9Ij6qpmb0hzDmwe6cIqq15I,6666
-pyshared-1.5.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyshared-1.5.2.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
-pyshared-1.5.2.dist-info/RECORD,,
+pyshared/version.py,sha256=mvQ7nJwcwEkbyD9OYSTfEPdWnrUwfgEf6kkbYY_zLqU,22
+pyshared-1.5.3.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
+pyshared-1.5.3.dist-info/METADATA,sha256=LmMfT2GjBVHI6ymjT8S9mRl3YwD2vfFJzH5yepCsSsM,6742
+pyshared-1.5.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyshared-1.5.3.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
+pyshared-1.5.3.dist-info/RECORD,,
```

