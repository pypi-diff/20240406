# Comparing `tmp/django_pgmigrate-1.3.0.tar.gz` & `tmp/django_pgmigrate-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgmigrate-1.3.0.tar", max compression
+gzip compressed data, was "django_pgmigrate-1.3.1.tar", max compression
```

## Comparing `django_pgmigrate-1.3.0.tar` & `django_pgmigrate-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1456 2023-11-26 23:00:55.285649 django_pgmigrate-1.3.0/LICENSE
--rw-r--r--   0        0        0     2739 2023-11-26 23:00:55.285649 django_pgmigrate-1.3.0/README.md
--rw-r--r--   0        0        0      320 2023-11-26 23:00:55.293649 django_pgmigrate-1.3.0/pgmigrate/__init__.py
--rw-r--r--   0        0        0     2147 2023-11-26 23:00:55.293649 django_pgmigrate-1.3.0/pgmigrate/action.py
--rw-r--r--   0        0        0      188 2023-11-26 23:00:55.293649 django_pgmigrate-1.3.0/pgmigrate/apps.py
--rw-r--r--   0        0        0     1065 2023-11-26 23:00:55.293649 django_pgmigrate-1.3.0/pgmigrate/config.py
--rw-r--r--   0        0        0      630 2023-11-26 23:00:55.293649 django_pgmigrate-1.3.0/pgmigrate/core.py
--rw-r--r--   0        0        0        0 2023-11-26 23:00:55.293649 django_pgmigrate-1.3.0/pgmigrate/management/__init__.py
--rw-r--r--   0        0        0        0 2023-11-26 23:00:55.293649 django_pgmigrate-1.3.0/pgmigrate/management/commands/__init__.py
--rw-r--r--   0        0        0     2262 2023-11-26 23:00:55.293649 django_pgmigrate-1.3.0/pgmigrate/management/commands/pgmigrate.py
--rw-r--r--   0        0        0       83 2023-11-26 23:00:55.293649 django_pgmigrate-1.3.0/pgmigrate/version.py
--rw-r--r--   0        0        0     2212 2023-11-26 23:01:44.117607 django_pgmigrate-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3990 1970-01-01 00:00:00.000000 django_pgmigrate-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-06 16:54:57.512436 django_pgmigrate-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2739 2024-04-06 16:54:57.512436 django_pgmigrate-1.3.1/README.md
+-rw-r--r--   0        0        0      320 2024-04-06 16:54:57.516436 django_pgmigrate-1.3.1/pgmigrate/__init__.py
+-rw-r--r--   0        0        0     2147 2024-04-06 16:54:57.516436 django_pgmigrate-1.3.1/pgmigrate/action.py
+-rw-r--r--   0        0        0      188 2024-04-06 16:54:57.516436 django_pgmigrate-1.3.1/pgmigrate/apps.py
+-rw-r--r--   0        0        0     1065 2024-04-06 16:54:57.516436 django_pgmigrate-1.3.1/pgmigrate/config.py
+-rw-r--r--   0        0        0      630 2024-04-06 16:54:57.516436 django_pgmigrate-1.3.1/pgmigrate/core.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:54:57.516436 django_pgmigrate-1.3.1/pgmigrate/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:54:57.516436 django_pgmigrate-1.3.1/pgmigrate/management/commands/__init__.py
+-rw-r--r--   0        0        0     2262 2024-04-06 16:54:57.516436 django_pgmigrate-1.3.1/pgmigrate/management/commands/pgmigrate.py
+-rw-r--r--   0        0        0       83 2024-04-06 16:54:57.516436 django_pgmigrate-1.3.1/pgmigrate/version.py
+-rw-r--r--   0        0        0     2212 2024-04-06 16:55:42.100666 django_pgmigrate-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3990 1970-01-01 00:00:00.000000 django_pgmigrate-1.3.1/PKG-INFO
```

### Comparing `django_pgmigrate-1.3.0/LICENSE` & `django_pgmigrate-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgmigrate-1.3.0/README.md` & `django_pgmigrate-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pgmigrate-1.3.0/pgmigrate/action.py` & `django_pgmigrate-1.3.1/pgmigrate/action.py`

 * *Files identical despite different names*

### Comparing `django_pgmigrate-1.3.0/pgmigrate/config.py` & `django_pgmigrate-1.3.1/pgmigrate/config.py`

 * *Files identical despite different names*

### Comparing `django_pgmigrate-1.3.0/pgmigrate/core.py` & `django_pgmigrate-1.3.1/pgmigrate/core.py`

 * *Files identical despite different names*

### Comparing `django_pgmigrate-1.3.0/pgmigrate/management/commands/pgmigrate.py` & `django_pgmigrate-1.3.1/pgmigrate/management/commands/pgmigrate.py`

 * *Files identical despite different names*

### Comparing `django_pgmigrate-1.3.0/pyproject.toml` & `django_pgmigrate-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pgmigrate"
 packages = [
   { include = "pgmigrate" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.3.0"
+version = "1.3.1"
 description = "Less downtime during migrations."
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_pgmigrate-1.3.0/PKG-INFO` & `django_pgmigrate-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgmigrate
-Version: 1.3.0
+Version: 1.3.1
 Summary: Less downtime during migrations.
 Home-page: https://github.com/Opus10/django-pgmigrate
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

