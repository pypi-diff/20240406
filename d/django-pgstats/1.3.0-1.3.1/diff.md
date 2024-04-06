# Comparing `tmp/django_pgstats-1.3.0.tar.gz` & `tmp/django_pgstats-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgstats-1.3.0.tar", max compression
+gzip compressed data, was "django_pgstats-1.3.1.tar", max compression
```

## Comparing `django_pgstats-1.3.0.tar` & `django_pgstats-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1456 2023-11-26 22:56:08.780512 django_pgstats-1.3.0/LICENSE
--rw-r--r--   0        0        0     1396 2023-11-26 22:56:08.780512 django_pgstats-1.3.0/README.md
--rw-r--r--   0        0        0       67 2023-11-26 22:56:08.780512 django_pgstats-1.3.0/pgstats/__init__.py
--rw-r--r--   0        0        0        0 2023-11-26 22:56:08.780512 django_pgstats-1.3.0/pgstats/management/__init__.py
--rw-r--r--   0        0        0        0 2023-11-26 22:56:08.780512 django_pgstats-1.3.0/pgstats/management/commands/__init__.py
--rw-r--r--   0        0        0      319 2023-11-26 22:56:08.780512 django_pgstats-1.3.0/pgstats/management/commands/snapshot_pgstats.py
--rw-r--r--   0        0        0     1638 2023-11-26 22:56:08.780512 django_pgstats-1.3.0/pgstats/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-11-26 22:56:08.780512 django_pgstats-1.3.0/pgstats/migrations/__init__.py
--rw-r--r--   0        0        0     1949 2023-11-26 22:56:08.780512 django_pgstats-1.3.0/pgstats/models.py
--rw-r--r--   0        0        0       81 2023-11-26 22:56:08.780512 django_pgstats-1.3.0/pgstats/version.py
--rw-r--r--   0        0        0     2187 2023-11-26 22:56:51.724743 django_pgstats-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2614 1970-01-01 00:00:00.000000 django_pgstats-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-06 16:49:36.553299 django_pgstats-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1396 2024-04-06 16:49:36.557299 django_pgstats-1.3.1/README.md
+-rw-r--r--   0        0        0       67 2024-04-06 16:49:36.557299 django_pgstats-1.3.1/pgstats/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:49:36.557299 django_pgstats-1.3.1/pgstats/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:49:36.557299 django_pgstats-1.3.1/pgstats/management/commands/__init__.py
+-rw-r--r--   0        0        0      319 2024-04-06 16:49:36.557299 django_pgstats-1.3.1/pgstats/management/commands/snapshot_pgstats.py
+-rw-r--r--   0        0        0     1638 2024-04-06 16:49:36.557299 django_pgstats-1.3.1/pgstats/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:49:36.557299 django_pgstats-1.3.1/pgstats/migrations/__init__.py
+-rw-r--r--   0        0        0     1949 2024-04-06 16:49:36.557299 django_pgstats-1.3.1/pgstats/models.py
+-rw-r--r--   0        0        0       81 2024-04-06 16:49:36.557299 django_pgstats-1.3.1/pgstats/version.py
+-rw-r--r--   0        0        0     2187 2024-04-06 16:51:30.749062 django_pgstats-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2614 1970-01-01 00:00:00.000000 django_pgstats-1.3.1/PKG-INFO
```

### Comparing `django_pgstats-1.3.0/LICENSE` & `django_pgstats-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgstats-1.3.0/README.md` & `django_pgstats-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pgstats-1.3.0/pgstats/migrations/0001_initial.py` & `django_pgstats-1.3.1/pgstats/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pgstats-1.3.0/pgstats/models.py` & `django_pgstats-1.3.1/pgstats/models.py`

 * *Files identical despite different names*

### Comparing `django_pgstats-1.3.0/pyproject.toml` & `django_pgstats-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pgstats"
 packages = [
   { include = "pgstats" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.3.0"
+version = "1.3.1"
 description = "Commands and models for tracking internal postgres stats."
 authors = ["Wes Kendall", "Tómas Árni Jónasson"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_pgstats-1.3.0/PKG-INFO` & `django_pgstats-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgstats
-Version: 1.3.0
+Version: 1.3.1
 Summary: Commands and models for tracking internal postgres stats.
 Home-page: https://github.com/Opus10/django-pgstats
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

