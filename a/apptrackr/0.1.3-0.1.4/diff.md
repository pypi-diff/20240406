# Comparing `tmp/apptrackr-0.1.3.tar.gz` & `tmp/apptrackr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.1.3.tar", max compression
+gzip compressed data, was "apptrackr-0.1.4.tar", max compression
```

## Comparing `apptrackr-0.1.3.tar` & `apptrackr-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.3/README.md
--rw-r--r--   0        0        0     5633 2024-04-05 14:44:34.320401 apptrackr-0.1.3/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.3/apptrackr/model/__init__.py
--rw-r--r--   0        0        0      688 2024-04-05 14:43:11.847544 apptrackr-0.1.3/apptrackr/model/model.py
--rw-r--r--   0        0        0      414 2024-04-05 14:45:06.671574 apptrackr-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 apptrackr-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.4/README.md
+-rw-r--r--   0        0        0     6278 2024-04-05 16:13:40.478649 apptrackr-0.1.4/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.4/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-05 14:43:11.847544 apptrackr-0.1.4/apptrackr/model/model.py
+-rw-r--r--   0        0        0      414 2024-04-05 16:15:36.314036 apptrackr-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 apptrackr-0.1.4/PKG-INFO
```

### Comparing `apptrackr-0.1.3/apptrackr/main.py` & `apptrackr-0.1.4/apptrackr/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Optional
 
 import typer
+from rich import box
+from rich.color import Color
+from rich.console import Console
+from rich.table import Table
 from typing_extensions import Annotated
 
-from .model import Applications
+from apptrackr.model import Applications
 
 tracker = typer.Typer()
+console = Console()
 
 
 @tracker.command()
 def count(
-    active: Annotated[
-        bool,
-        typer.Option(
-            help="Get only active application",
-        ),
-    ] = False
+    active: Annotated[bool, typer.Option(help="Get only active application")] = False
 ) -> None:
     """
     Fetch counts of applications.
 
     Args:
         active (Annotated[ bool, typer.Option, optional): Fetch only active applications.)]=False.
     """
@@ -50,17 +50,17 @@
 ) -> None:
     """Add new application to the database.
 
     Args:
         name (Annotated[str, typer.Argument, optional): Job application name)].
         status (Annotated[str, typer.Argument, optional): Job status)].
         apply_link (Annotated[str, typer.Argument, optional): Application link)].
+        applied_through (Annotated[str], typer.Argument, optional): Optional Application date)].
         location (Annotated[ Optional[str], typer.Argument, optional): Optional Job location)]=None.
-        date (Annotated[ Optional[str], typer.Argument, optional): Optional Application date)]=None.
-
+        date (Annotated[ Optional[str], typer.Argument, optional): Optional Application date)]=None.:
     Raises:
         typer.Exit: For invalid arguments
     """
     if status not in ("active", "rejected", "accepted"):
         typer.echo("Invalid status argument!")
         raise typer.Exit(-1)
 
@@ -111,35 +111,51 @@
     columns = {
         "name": name,
         "status": status,
         "location": location,
         "date": date,
         "apply_link": apply_link,
     }
-    per_page = 10
 
+    per_page = 10
     for k, v in columns.items():
         if v:
             filters.append(getattr(Applications, k) == v)
 
     applications = (
         Applications.select().where(*filters).paginate(page_number or 1, per_page)
         if filters
         else Applications.select().paginate(page_number or 1, per_page)
     )
+    table = Table(
+        "ID", "Name", "Status", "Location", "Date", "Application Link", box=box.MINIMAL
+    )
     for application in applications:
-        print(
-            application.application_id,
+        match application.status:
+            case "rejected":
+                style = "red on black"
+            case "active":
+                style = "yellow"
+            case "accepted":
+                style = "green"
+            case _:
+                style = "white"
+
+        table.add_row(
+            str(application.application_id),
             application.name,
             application.status,
             application.location,
             application.date,
             application.apply_link,
+            style=style,
         )
 
+    console.print(table)
+
 
 @tracker.command()
 def delete_application(
     name: Optional[str] = typer.Option(
         None, "--name", "-n", help="Name of the application"
     ),
     application_id: Optional[str] = typer.Option(
```

### Comparing `apptrackr-0.1.3/apptrackr/model/model.py` & `apptrackr-0.1.4/apptrackr/model/model.py`

 * *Files identical despite different names*

