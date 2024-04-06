# Comparing `tmp/flask_dbmigrant-1.0.0.tar.gz` & `tmp/flask_dbmigrant-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_dbmigrant-1.0.0.tar", max compression
+gzip compressed data, was "flask_dbmigrant-1.0.1.tar", max compression
```

## Comparing `flask_dbmigrant-1.0.0.tar` & `flask_dbmigrant-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2024-01-10 07:41:45.546746 flask_dbmigrant-1.0.0/LICENSE
--rw-r--r--   0        0        0     1010 2024-03-30 12:10:41.531388 flask_dbmigrant-1.0.0/README.md
--rw-r--r--   0        0        0      420 2024-03-30 12:14:01.787373 flask_dbmigrant-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2483 2024-03-30 11:51:19.701204 flask_dbmigrant-1.0.0/src/flask_dbmigrant/__init__.py
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 flask_dbmigrant-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-10 07:41:45.546746 flask_dbmigrant-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1010 2024-03-30 12:10:41.531388 flask_dbmigrant-1.0.1/README.md
+-rw-r--r--   0        0        0      420 2024-04-06 09:28:59.693028 flask_dbmigrant-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2484 2024-04-06 09:27:50.058183 flask_dbmigrant-1.0.1/src/flask_dbmigrant/__init__.py
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 flask_dbmigrant-1.0.1/PKG-INFO
```

### Comparing `flask_dbmigrant-1.0.0/LICENSE` & `flask_dbmigrant-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_dbmigrant-1.0.0/README.md` & `flask_dbmigrant-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `flask_dbmigrant-1.0.0/src/flask_dbmigrant/__init__.py` & `flask_dbmigrant-1.0.1/src/flask_dbmigrant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class DbMigrant:
     def __init__(self, app=None):
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app):
-        DB_MODULE = app.config["DB_MODEL"]
+        DB_MODULE = app.config["DB_MODULE"]
         DATABASE_URL = app.config["DATABASE_URL"]
 
         @app.cli.command("db")
         @click.argument("command")
         def db_command(command):
             """Possible commands:
```

### Comparing `flask_dbmigrant-1.0.0/PKG-INFO` & `flask_dbmigrant-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-dbmigrant
-Version: 1.0.0
+Version: 1.0.1
 Summary: Flask extension for working with Alembic
 Author: Rafal Padkowski
 Author-email: rafaelp@poczta.onet.pl
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

