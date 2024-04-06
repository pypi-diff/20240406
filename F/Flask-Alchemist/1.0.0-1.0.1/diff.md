# Comparing `tmp/flask_alchemist-1.0.0.tar.gz` & `tmp/flask_alchemist-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_alchemist-1.0.0.tar", max compression
+gzip compressed data, was "flask_alchemist-1.0.1.tar", max compression
```

## Comparing `flask_alchemist-1.0.0.tar` & `flask_alchemist-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2024-01-10 07:41:45.546746 flask_alchemist-1.0.0/LICENSE
--rw-r--r--   0        0        0     3230 2024-02-21 12:28:49.985440 flask_alchemist-1.0.0/README.md
--rw-r--r--   0        0        0      473 2024-02-21 12:11:36.697719 flask_alchemist-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6661 2024-02-21 12:35:26.968778 flask_alchemist-1.0.0/src/flask_alchemist/__init__.py
--rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 flask_alchemist-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-10 07:41:45.546746 flask_alchemist-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2933 2024-04-06 08:43:37.197159 flask_alchemist-1.0.1/README.md
+-rw-r--r--   0        0        0      461 2024-04-06 08:44:07.608994 flask_alchemist-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4374 2024-04-06 08:37:20.835017 flask_alchemist-1.0.1/src/flask_alchemist/__init__.py
+-rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 flask_alchemist-1.0.1/PKG-INFO
```

### Comparing `flask_alchemist-1.0.0/LICENSE` & `flask_alchemist-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_alchemist-1.0.0/README.md` & `flask_alchemist-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,30 @@
+Metadata-Version: 2.1
+Name: Flask-Alchemist
+Version: 1.0.1
+Summary: Flask extension for working with SQLAlchemy
+License: MIT
+Author: Rafal Padkowski
+Author-email: rafaelp@poczta.onet.pl
+Requires-Python: >=3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: alembic (>=1.13.0)
+Requires-Dist: flask (>=3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.0)
+Description-Content-Type: text/markdown
+
 # Flask-Alchemist
 
-Flask extension for working with SQLAlchemy and Alembic.
+Flask extension for working with SQLAlchemy.
 
-It can be used as an alternative for Flask-SQLAlchemy and Flask-Migrate.
+It can be used as an alternative for Flask-SQLAlchemy.
 
 Instead of the scoped session tied to a thread you can instantiate database session
 on demand with a context manager. The advantage is that when the Flask application handles a request you can precisely control when the session starts and ends.
 
 There is also a Model class with modified MetaData configuration which tells SQLAlchemy how to name indexes and constraints in a database.
 You can subclass it to define your own model classes.
 
@@ -77,27 +95,13 @@
 ## Other features
 
 Alchemist object can be used as a proxy for any attribute of the SQLAlchemy Core and the SQLAlchemy ORM.
 For example when making SQL queries you can use db.select instead of importing this from SQLAlchemy.
 
 There is also a Pagination class for paging query results (similar to Flask-SQLAlchemy).
 
-There are couple commands to work with Alembic:
-- flask db init
-
-  create a migration repository and configure the environment
-
-- flask db migrate
-
-  create a migration script
-
-- flask db upgrade
-
-  execute the script
-
-The app package should contain models.py file.
-
 
 ## License
 
 `Flask-Alchemist` was created by Rafal Padkowski. It is licensed under the terms
 of the MIT license.
+
```

### Comparing `flask_alchemist-1.0.0/PKG-INFO` & `flask_alchemist-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-Metadata-Version: 2.1
-Name: Flask-Alchemist
-Version: 1.0.0
-Summary: Flask extension for working with SQLAlchemy and Alembic
-License: MIT
-Author: Rafal Padkowski
-Author-email: rafaelp@poczta.onet.pl
-Requires-Python: >=3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: alembic (>=1.13.0)
-Requires-Dist: flask (>=3.0.0)
-Requires-Dist: sqlalchemy (>=2.0.0)
-Description-Content-Type: text/markdown
-
 # Flask-Alchemist
 
-Flask extension for working with SQLAlchemy and Alembic.
+Flask extension for working with SQLAlchemy.
 
-It can be used as an alternative for Flask-SQLAlchemy and Flask-Migrate.
+It can be used as an alternative for Flask-SQLAlchemy.
 
 Instead of the scoped session tied to a thread you can instantiate database session
 on demand with a context manager. The advantage is that when the Flask application handles a request you can precisely control when the session starts and ends.
 
 There is also a Model class with modified MetaData configuration which tells SQLAlchemy how to name indexes and constraints in a database.
 You can subclass it to define your own model classes.
 
@@ -95,28 +77,12 @@
 ## Other features
 
 Alchemist object can be used as a proxy for any attribute of the SQLAlchemy Core and the SQLAlchemy ORM.
 For example when making SQL queries you can use db.select instead of importing this from SQLAlchemy.
 
 There is also a Pagination class for paging query results (similar to Flask-SQLAlchemy).
 
-There are couple commands to work with Alembic:
-- flask db init
-
-  create a migration repository and configure the environment
-
-- flask db migrate
-
-  create a migration script
-
-- flask db upgrade
-
-  execute the script
-
-The app package should contain models.py file.
-
 
 ## License
 
 `Flask-Alchemist` was created by Rafal Padkowski. It is licensed under the terms
 of the MIT license.
-
```

