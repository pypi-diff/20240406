# Comparing `tmp/apptrackr-0.1.6.tar.gz` & `tmp/apptrackr-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.1.6.tar", max compression
+gzip compressed data, was "apptrackr-0.1.7.tar", max compression
```

## Comparing `apptrackr-0.1.6.tar` & `apptrackr-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.6/README.md
--rw-r--r--   0        0        0      157 2024-04-06 06:14:00.743036 apptrackr-0.1.6/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.6/apptrackr/model/__init__.py
--rw-r--r--   0        0        0      769 2024-04-06 05:50:41.837541 apptrackr-0.1.6/apptrackr/model/model.py
--rw-r--r--   0        0        0        0 2024-04-06 07:52:37.461768 apptrackr-0.1.6/apptrackr/modules/gen.py
--rw-r--r--   0        0        0     9184 2024-04-06 08:34:51.080809 apptrackr-0.1.6/apptrackr/modules/storage.py
--rw-r--r--   0        0        0      454 2024-04-06 08:35:21.663756 apptrackr-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 apptrackr-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.7/README.md
+-rw-r--r--   0        0        0      303 2024-04-06 10:55:26.554890 apptrackr-0.1.7/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.7/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0     1449 2024-04-06 10:54:21.271269 apptrackr-0.1.7/apptrackr/model/migrations.py
+-rw-r--r--   0        0        0       31 2024-04-06 10:50:49.114231 apptrackr-0.1.7/apptrackr/model/migrations.txt
+-rw-r--r--   0        0        0      767 2024-04-06 10:17:28.998913 apptrackr-0.1.7/apptrackr/model/model.py
+-rw-r--r--   0        0        0      833 2024-04-06 09:22:12.817203 apptrackr-0.1.7/apptrackr/modules/sources.py
+-rw-r--r--   0        0        0       95 2024-04-06 10:10:55.875981 apptrackr-0.1.7/apptrackr/modules/status.py
+-rw-r--r--   0        0        0     9172 2024-04-06 10:52:29.213958 apptrackr-0.1.7/apptrackr/modules/storage.py
+-rw-r--r--   0        0        0      454 2024-04-06 10:57:33.830142 apptrackr-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 apptrackr-0.1.7/PKG-INFO
```

### Comparing `apptrackr-0.1.6/apptrackr/model/model.py` & `apptrackr-0.1.7/apptrackr/model/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class Applications(Model):
     application_id = AutoField()
     name = CharField(max_length=100)
     status = CharField()
     location = CharField(default="uk")
     date = DateTimeField(formats="%d/%m/%y %H:%M:%S.%f", default=datetime.now)
     apply_link = CharField(max_length=150)
-    applied_through = CharField()
+    email_id_used = CharField()
 
     class Meta:
         database = database
 
 
 if not Applications.table_exists():
     print("Creating Application Table...")
```

### Comparing `apptrackr-0.1.6/apptrackr/modules/storage.py` & `apptrackr-0.1.7/apptrackr/modules/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 @storage.command()
 def add_application(
     name: Annotated[str, typer.Argument(help="Job application name")],
     status: Annotated[str, typer.Argument(help="Job status")],
     apply_link: Annotated[str, typer.Argument(help="Application link")],
-    applied_through: Annotated[
+    email_id_used: Annotated[
         str, typer.Argument(help="Email Id sent with application")
     ],
     location: Annotated[
         Optional[str], typer.Argument(help="Optional Job location")
     ] = None,
     date: Annotated[
         Optional[str], typer.Argument(help="Optional Application date")
@@ -50,29 +50,29 @@
 ) -> None:
     """Add new application to the database.
 
     Args:
         name (Annotated[str, typer.Argument, optional): Job application name)].
         status (Annotated[str, typer.Argument, optional): Job status)].
         apply_link (Annotated[str, typer.Argument, optional): Application link)].
-        applied_through (Annotated[str], typer.Argument, optional): Optional Application date)].
+        email_id_used (Annotated[str], typer.Argument, optional): Optional Application date)].
         location (Annotated[ Optional[str], typer.Argument, optional): Optional Job location)]=None.
         date (Annotated[ Optional[str], typer.Argument, optional): Optional Application date)]=None.:
     Raises:
         typer.Exit: For invalid arguments
     """
     if status not in ("active", "rejected", "accepted"):
         typer.echo("Invalid status argument!")
         raise typer.Exit(-1)
 
     application_details = {
         "name": name,
         "status": status,
         "apply_link": apply_link,
-        "applied_through": applied_through,
+        "email_id_used": email_id_used,
     }
 
     if location:
         application_details["location"] = location
 
     if date:
         application_details["date"] = date
@@ -144,15 +144,15 @@
     table = Table(
         "ID",
         "Name",
         "Status",
         "Location",
         "Date",
         "Application Link",
-        "Applied Through",
+        "Email Id Used",
         box=box.MINIMAL,
     )
     for application in applications:
         match application.status:
             case "rejected":
                 style = "red on black"
             case "active":
@@ -165,15 +165,15 @@
         table.add_row(
             str(application.application_id),
             application.name,
             application.status,
             application.location,
             application.date,
             application.apply_link,
-            application.applied_through,
+            application.email_id_used,
             style=style,
         )
 
     console.print(table)
 
 
 @storage.command()
```

### Comparing `apptrackr-0.1.6/PKG-INFO` & `apptrackr-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apptrackr
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: MIT
 Author: Aradhya Tripathi
 Author-email: 67282231+Aradhya-Tripathi@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

