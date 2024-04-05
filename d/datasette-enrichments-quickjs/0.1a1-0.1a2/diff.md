# Comparing `tmp/datasette-enrichments-quickjs-0.1a1.tar.gz` & `tmp/datasette-enrichments-quickjs-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-enrichments-quickjs-0.1a1.tar", last modified: Sat Mar  9 14:57:15 2024, max compression
+gzip compressed data, was "datasette-enrichments-quickjs-0.1a2.tar", last modified: Fri Apr  5 22:08:15 2024, max compression
```

## Comparing `datasette-enrichments-quickjs-0.1a1.tar` & `datasette-enrichments-quickjs-0.1a2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 14:57:15.352353 datasette-enrichments-quickjs-0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-09 14:57:07.000000 datasette-enrichments-quickjs-0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-03-09 14:57:15.352353 datasette-enrichments-quickjs-0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-09 14:57:07.000000 datasette-enrichments-quickjs-0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 14:57:15.348353 datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs/
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-03-09 14:57:07.000000 datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 14:57:15.352353 datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-03-09 14:57:15.000000 datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-09 14:57:15.000000 datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 14:57:15.000000 datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-09 14:57:15.000000 datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-09 14:57:15.000000 datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-09 14:57:15.000000 datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-09 14:57:07.000000 datasette-enrichments-quickjs-0.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 14:57:15.352353 datasette-enrichments-quickjs-0.1a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 14:57:15.352353 datasette-enrichments-quickjs-0.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-03-09 14:57:07.000000 datasette-enrichments-quickjs-0.1a1/tests/test_enrichments_quickjs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:08:15.257321 datasette-enrichments-quickjs-0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 22:08:08.000000 datasette-enrichments-quickjs-0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-05 22:08:15.257321 datasette-enrichments-quickjs-0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-05 22:08:08.000000 datasette-enrichments-quickjs-0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:08:15.253321 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-05 22:08:08.000000 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:08:15.257321 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-05 22:08:08.000000 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs/templates/enrichment-quickjs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:08:15.257321 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-05 22:08:15.000000 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-05 22:08:15.000000 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 22:08:15.000000 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 22:08:15.000000 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 22:08:15.000000 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 22:08:15.000000 datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-05 22:08:08.000000 datasette-enrichments-quickjs-0.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 22:08:15.257321 datasette-enrichments-quickjs-0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:08:15.257321 datasette-enrichments-quickjs-0.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-04-05 22:08:08.000000 datasette-enrichments-quickjs-0.1a2/tests/test_enrichments_quickjs.py
```

### Comparing `datasette-enrichments-quickjs-0.1a1/LICENSE` & `datasette-enrichments-quickjs-0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-quickjs-0.1a1/PKG-INFO` & `datasette-enrichments-quickjs-0.1a2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments-quickjs
-Version: 0.1a1
+Version: 0.1a2
 Summary: Enrich data with a custom JavaScript function
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-enrichments-quickjs
 Project-URL: Changelog, https://github.com/datasette/datasette-enrichments-quickjs/releases
 Project-URL: Issues, https://github.com/datasette/datasette-enrichments-quickjs/issues
 Project-URL: CI, https://github.com/datasette/datasette-enrichments-quickjs/actions
@@ -46,14 +46,30 @@
 Enrichment JavaScript functions look like this:
 
 ```javascript
 function enrich(row) {
     return row["title"] + "!";
 }
 ```
+The return value of your function will be stored in the output column of your choice.
+
+Instead of picking an output column, you can have your function return an object with keys and values.
+
+This example takes a `point` column with values like `37.7749,-122.4194 and splits it into `latitude` and `longitude` columns:
+
+```javascript
+function enrich(row) {
+    const bits = row.point.split(",");
+    return {
+        "latitude": parseFloat(bits[0]),
+        "longitude": parseFloat(bits[1])
+    }
+}
+```
+The enrichment will then create new columns in the table for each key in the object returned by that function.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-enrichments-quickjs
 python3 -m venv venv
```

### Comparing `datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs/__init__.py` & `datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datasette_enrichments import Enrichment
 from datasette import hookimpl
+import json
 import markupsafe
 from quickjs import Function
 import sqlite_utils
 from wtforms import Form, StringField, TextAreaField, SelectField, ValidationError
 from wtforms.validators import DataRequired
 
 
@@ -15,14 +16,17 @@
 class QuickJsEnrichment(Enrichment):
     name = "JavaScript"
     slug = "quickjs"
     description = "Enrich data with a custom JavaScript function"
 
     async def initialize(self, datasette, db, table, config):
         # Ensure column exists
+        if config["mode"] == "multi":
+            # No need to create columns for multi mode
+            return
         output_column = config["output_column"]
         column_type = config["output_column_type"].upper()
 
         def add_column_if_not_exists(conn):
             db = sqlite_utils.Database(conn)
             if output_column not in db[table].columns_dict:
                 db[table].add_column(output_column, column_type)
@@ -41,14 +45,25 @@
                 "JavaScript function",
                 description=markupsafe.Markup(
                     "<br>".join(markupsafe.escape(bit) for bit in bits)
                 ),
                 validators=[DataRequired(message="JavaScript function is required.")],
                 default='function enrich(row) {\n  return JSON.stringify(row) + " enriched";\n}',
             )
+            mode = SelectField(
+                "Output mode",
+                choices=[
+                    ("single", "Store the function result in a single column"),
+                    (
+                        "multi",
+                        "Return an object and store each key in a separate column",
+                    ),
+                ],
+                validators=[DataRequired(message="A mode is required.")],
+            )
             output_column = StringField(
                 "Output column name",
                 description="The column to store the output in - will be created if it does not exist.",
                 validators=[DataRequired(message="Column is required.")],
                 default="javascript_output",
             )
             output_column_type = SelectField(
@@ -80,20 +95,34 @@
         config,
     ):
         function = Function("enrich", config["javascript"])
         function.set_time_limit(0.1)  # 0.1s
         function.set_memory_limit(4 * 1024 * 1024)  # 4MB
         output_column = config["output_column"]
         for row in rows:
-            try:
-                output = function(row)
-            except Exception as ex:
-                print(ex, repr(ex))
-                raise
-            await db.execute_write(
-                "update [{table}] set [{output_column}] = ? where {wheres}".format(
-                    table=table,
-                    output_column=output_column,
-                    wheres=" and ".join('"{}" = ?'.format(pk) for pk in pks),
-                ),
-                [output] + list(row[pk] for pk in pks),
-            )
+            output = function(row)
+            if config["mode"] == "multi":
+                if isinstance(output, str) and not isinstance(output, dict):
+                    try:
+                        output = json.loads(output)
+                    except json.JSONDecodeError:
+                        output = {"javascript_output": output}
+                if len(pks) == 1:
+                    pk_value = row[pks[0]]
+                else:
+                    pk_value = (row[pk] for pk in pks)
+
+                def _update(conn):
+                    sqlite_utils.Database(conn)[table].update(
+                        pk_value, output, alter=True
+                    )
+
+                await db.execute_write_fn(_update)
+            else:
+                await db.execute_write(
+                    "update [{table}] set [{output_column}] = ? where {wheres}".format(
+                        table=table,
+                        output_column=output_column,
+                        wheres=" and ".join('"{}" = ?'.format(pk) for pk in pks),
+                    ),
+                    [output] + list(row[pk] for pk in pks),
+                )
```

### Comparing `datasette-enrichments-quickjs-0.1a1/datasette_enrichments_quickjs.egg-info/PKG-INFO` & `datasette-enrichments-quickjs-0.1a2/datasette_enrichments_quickjs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments-quickjs
-Version: 0.1a1
+Version: 0.1a2
 Summary: Enrich data with a custom JavaScript function
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-enrichments-quickjs
 Project-URL: Changelog, https://github.com/datasette/datasette-enrichments-quickjs/releases
 Project-URL: Issues, https://github.com/datasette/datasette-enrichments-quickjs/issues
 Project-URL: CI, https://github.com/datasette/datasette-enrichments-quickjs/actions
@@ -46,14 +46,30 @@
 Enrichment JavaScript functions look like this:
 
 ```javascript
 function enrich(row) {
     return row["title"] + "!";
 }
 ```
+The return value of your function will be stored in the output column of your choice.
+
+Instead of picking an output column, you can have your function return an object with keys and values.
+
+This example takes a `point` column with values like `37.7749,-122.4194 and splits it into `latitude` and `longitude` columns:
+
+```javascript
+function enrich(row) {
+    const bits = row.point.split(",");
+    return {
+        "latitude": parseFloat(bits[0]),
+        "longitude": parseFloat(bits[1])
+    }
+}
+```
+The enrichment will then create new columns in the table for each key in the object returned by that function.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-enrichments-quickjs
 python3 -m venv venv
```

### Comparing `datasette-enrichments-quickjs-0.1a1/pyproject.toml` & `datasette-enrichments-quickjs-0.1a2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-enrichments-quickjs"
-version = "0.1a1"
+version = "0.1a2"
 description = "Enrich data with a custom JavaScript function"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
@@ -27,7 +27,10 @@
 enrichments_quickjs = "datasette_enrichments_quickjs"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-asyncio", "pytest-timeout"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
+
+[tool.setuptools.package-data]
+datasette_enrichments_quickjs = ["templates/*"]
```

### Comparing `datasette-enrichments-quickjs-0.1a1/tests/test_enrichments_quickjs.py` & `datasette-enrichments-quickjs-0.1a2/tests/test_enrichments_quickjs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 from datasette.app import Datasette
+import json
 import pytest
 import sqlite_utils
 
 
 async def _cookies(datasette, path="/-/enrich/data/items/quickjs"):
     cookies = {"ds_actor": datasette.sign({"a": {"id": "root"}}, "actor")}
     csrftoken = (await datasette.client.get(path, cookies=cookies)).cookies[
@@ -24,14 +25,15 @@
         {"id": 3, "name": "Three", "description": "Third item"},
     ]
     db["items"].insert_all(rows, pk="id")
 
     cookies = await _cookies(datasette)
     post = {
         "javascript": "function enrich(row) { return row.description.length }",
+        "mode": "single",
         "output_column": "description_length",
         "output_column_type": "integer",
     }
     post["csrftoken"] = cookies["ds_csrftoken"]
     response = await datasette.client.post(
         "/-/enrich/data/items/quickjs",
         data=post,
@@ -61,14 +63,80 @@
             "description": "Third item",
             "description_length": 10,
         },
     ]
 
 
 @pytest.mark.asyncio
+async def test_enrichment_multi(tmpdir):
+    data = str(tmpdir / "data.db")
+    datasette = Datasette([data], memory=True)
+    db = sqlite_utils.Database(data)
+    rows = [
+        {
+            "id": 1,
+            "name": "NYC",
+            "point": "40.71,-74.0",
+        },
+        {
+            "id": 2,
+            "name": "SF",
+            "point": "37.77,-122.41",
+        },
+    ]
+    db["items"].insert_all(rows, pk="id")
+
+    cookies = await _cookies(datasette)
+    post = {
+        "javascript": """
+            function enrich(row) {
+                const bits = row.point.split(",");
+                return {
+                    "latitude": parseFloat(bits[0]),
+                    "longitude": parseFloat(bits[1])
+                }
+            }
+        """,
+        "mode": "multi",
+    }
+    post["csrftoken"] = cookies["ds_csrftoken"]
+    response = await datasette.client.post(
+        "/-/enrich/data/items/quickjs",
+        data=post,
+        cookies=cookies,
+    )
+    assert response.status_code == 302
+    await asyncio.sleep(0.3)
+    db = datasette.get_database("data")
+    jobs = await db.execute("select * from _enrichment_jobs")
+    job = dict(jobs.first())
+    assert job["status"] == "finished"
+    assert job["enrichment"] == "quickjs"
+    assert job["done_count"] == 2
+    results = await db.execute("select * from items order by id")
+    rows = [dict(r) for r in results.rows]
+    assert rows == [
+        {
+            "id": 1,
+            "name": "NYC",
+            "point": "40.71,-74.0",
+            "latitude": 40.71,
+            "longitude": -74.0,
+        },
+        {
+            "id": 2,
+            "name": "SF",
+            "point": "37.77,-122.41",
+            "latitude": 37.77,
+            "longitude": -122.41,
+        },
+    ]
+
+
+@pytest.mark.asyncio
 @pytest.mark.timeout(5)
 @pytest.mark.parametrize(
     "javascript,expected_error",
     [
         # Deeply nested object should run out of memory
         (
             """
@@ -120,14 +188,15 @@
     rows = [
         {"id": 1, "name": "One", "description": "First item"},
         {"id": 2, "name": "Two", "description": "Second item"},
         {"id": 3, "name": "Three", "description": "Third item"},
     ]
     post = {
         "javascript": javascript,
+        "mode": "single",
         "output_column": "description_length",
         "output_column_type": "integer",
     }
     post["csrftoken"] = cookies["ds_csrftoken"]
     response = await ds.client.post(
         "/-/enrich/test_time_and_memory_limit/foo/quickjs",
         data=post,
```

