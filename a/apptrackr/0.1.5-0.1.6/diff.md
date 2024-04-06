# Comparing `tmp/apptrackr-0.1.5.tar.gz` & `tmp/apptrackr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.1.5.tar", max compression
+gzip compressed data, was "apptrackr-0.1.6.tar", max compression
```

## Comparing `apptrackr-0.1.5.tar` & `apptrackr-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.5/README.md
--rw-r--r--   0        0        0      157 2024-04-06 06:14:00.743036 apptrackr-0.1.5/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.5/apptrackr/model/__init__.py
--rw-r--r--   0        0        0      769 2024-04-06 05:50:41.837541 apptrackr-0.1.5/apptrackr/model/model.py
--rw-r--r--   0        0        0        0 2024-04-05 17:20:29.132098 apptrackr-0.1.5/apptrackr/modules/gen.py
--rw-r--r--   0        0        0     9067 2024-04-06 06:16:00.719001 apptrackr-0.1.5/apptrackr/modules/storage.py
--rw-r--r--   0        0        0      454 2024-04-06 06:18:02.491176 apptrackr-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 apptrackr-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.6/README.md
+-rw-r--r--   0        0        0      157 2024-04-06 06:14:00.743036 apptrackr-0.1.6/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.6/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0      769 2024-04-06 05:50:41.837541 apptrackr-0.1.6/apptrackr/model/model.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:52:37.461768 apptrackr-0.1.6/apptrackr/modules/gen.py
+-rw-r--r--   0        0        0     9184 2024-04-06 08:34:51.080809 apptrackr-0.1.6/apptrackr/modules/storage.py
+-rw-r--r--   0        0        0      454 2024-04-06 08:35:21.663756 apptrackr-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 apptrackr-0.1.6/PKG-INFO
```

### Comparing `apptrackr-0.1.5/apptrackr/model/model.py` & `apptrackr-0.1.6/apptrackr/model/model.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.1.5/apptrackr/modules/storage.py` & `apptrackr-0.1.6/apptrackr/modules/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,22 @@
 
     applications = (
         Applications.select().where(*filters).paginate(page_number or 1, per_page)
         if filters
         else Applications.select().paginate(page_number or 1, per_page)
     )
     table = Table(
-        "ID", "Name", "Status", "Location", "Date", "Application Link", box=box.MINIMAL
+        "ID",
+        "Name",
+        "Status",
+        "Location",
+        "Date",
+        "Application Link",
+        "Applied Through",
+        box=box.MINIMAL,
     )
     for application in applications:
         match application.status:
             case "rejected":
                 style = "red on black"
             case "active":
                 style = "yellow"
@@ -158,14 +165,15 @@
         table.add_row(
             str(application.application_id),
             application.name,
             application.status,
             application.location,
             application.date,
             application.apply_link,
+            application.applied_through,
             style=style,
         )
 
     console.print(table)
 
 
 @storage.command()
```

### Comparing `apptrackr-0.1.5/PKG-INFO` & `apptrackr-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apptrackr
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: MIT
 Author: Aradhya Tripathi
 Author-email: 67282231+Aradhya-Tripathi@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

