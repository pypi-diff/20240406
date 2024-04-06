# Comparing `tmp/flask_dbmigrant-1.0.1.tar.gz` & `tmp/flask_dbmigrant-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_dbmigrant-1.0.1.tar", max compression
+gzip compressed data, was "flask_dbmigrant-1.0.2.tar", max compression
```

## Comparing `flask_dbmigrant-1.0.1.tar` & `flask_dbmigrant-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2024-01-10 07:41:45.546746 flask_dbmigrant-1.0.1/LICENSE
--rw-r--r--   0        0        0     1010 2024-03-30 12:10:41.531388 flask_dbmigrant-1.0.1/README.md
--rw-r--r--   0        0        0      420 2024-04-06 09:28:59.693028 flask_dbmigrant-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2484 2024-04-06 09:27:50.058183 flask_dbmigrant-1.0.1/src/flask_dbmigrant/__init__.py
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 flask_dbmigrant-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-10 07:41:45.546746 flask_dbmigrant-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1010 2024-03-30 12:10:41.531388 flask_dbmigrant-1.0.2/README.md
+-rw-r--r--   0        0        0      420 2024-04-06 09:51:46.971572 flask_dbmigrant-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2486 2024-04-06 09:50:24.592912 flask_dbmigrant-1.0.2/src/flask_dbmigrant/__init__.py
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 flask_dbmigrant-1.0.2/PKG-INFO
```

### Comparing `flask_dbmigrant-1.0.1/LICENSE` & `flask_dbmigrant-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_dbmigrant-1.0.1/README.md` & `flask_dbmigrant-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_dbmigrant-1.0.1/src/flask_dbmigrant/__init__.py` & `flask_dbmigrant-1.0.2/src/flask_dbmigrant/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                             if "target_metadata = None" in line:
                                 print(
                                     line.rstrip().replace(
                                         "None", f"{DB_MODULE}.metadata"
                                     )
                                 )
                                 print(
-                                    f'config.set_main_option("sqlalchemy.url", {DATABASE_URL})'
+                                    f'config.set_main_option("sqlalchemy.url", "{DATABASE_URL}")'
                                 )
                             elif (
                                 "connection=connection, target_metadata=target_metadata"
                                 in line
                             ):
                                 print(line.rstrip() + ", render_as_batch=True")
                             else:
```

### Comparing `flask_dbmigrant-1.0.1/PKG-INFO` & `flask_dbmigrant-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-dbmigrant
-Version: 1.0.1
+Version: 1.0.2
 Summary: Flask extension for working with Alembic
 Author: Rafal Padkowski
 Author-email: rafaelp@poczta.onet.pl
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

