# Comparing `tmp/apptrackr-0.1.4.tar.gz` & `tmp/apptrackr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.1.4.tar", max compression
+gzip compressed data, was "apptrackr-0.1.5.tar", max compression
```

## Comparing `apptrackr-0.1.4.tar` & `apptrackr-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.4/README.md
--rw-r--r--   0        0        0     6278 2024-04-05 16:13:40.478649 apptrackr-0.1.4/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.4/apptrackr/model/__init__.py
--rw-r--r--   0        0        0      688 2024-04-05 14:43:11.847544 apptrackr-0.1.4/apptrackr/model/model.py
--rw-r--r--   0        0        0      414 2024-04-05 16:15:36.314036 apptrackr-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 apptrackr-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.5/README.md
+-rw-r--r--   0        0        0      157 2024-04-06 06:14:00.743036 apptrackr-0.1.5/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.5/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0      769 2024-04-06 05:50:41.837541 apptrackr-0.1.5/apptrackr/model/model.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:20:29.132098 apptrackr-0.1.5/apptrackr/modules/gen.py
+-rw-r--r--   0        0        0     9067 2024-04-06 06:16:00.719001 apptrackr-0.1.5/apptrackr/modules/storage.py
+-rw-r--r--   0        0        0      454 2024-04-06 06:18:02.491176 apptrackr-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 apptrackr-0.1.5/PKG-INFO
```

### Comparing `apptrackr-0.1.4/apptrackr/model/model.py` & `apptrackr-0.1.5/apptrackr/model/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import os
 from datetime import datetime
 
 from peewee import AutoField, CharField, DateTimeField, Model, SqliteDatabase
 
 database = SqliteDatabase(
-    os.path.join(os.path.expanduser("~"), "applications.db"),
+    (
+        os.path.join(os.path.expanduser("~"), "applications.db")
+        if not os.getenv("dev")
+        else "./applications.db"
+    ),
 )
 
 
 class Applications(Model):
     application_id = AutoField()
     name = CharField(max_length=100)
     status = CharField()
```

