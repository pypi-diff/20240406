# Comparing `tmp/django_migration_docs-1.2.0.tar.gz` & `tmp/django_migration_docs-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_migration_docs-1.2.0.tar", max compression
+gzip compressed data, was "django_migration_docs-1.2.1.tar", max compression
```

## Comparing `django_migration_docs-1.2.0.tar` & `django_migration_docs-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1456 2023-11-26 22:45:29.596140 django_migration_docs-1.2.0/LICENSE
--rw-r--r--   0        0        0     1933 2023-11-26 22:45:29.596140 django_migration_docs-1.2.0/README.md
--rw-r--r--   0        0        0      419 2023-11-26 22:45:29.600140 django_migration_docs-1.2.0/migration_docs/__init__.py
--rw-r--r--   0        0        0     1118 2023-11-26 22:45:29.600140 django_migration_docs-1.2.0/migration_docs/apps.py
--rw-r--r--   0        0        0    16437 2023-11-26 22:45:29.600140 django_migration_docs-1.2.0/migration_docs/core.py
--rw-r--r--   0        0        0        0 2023-11-26 22:45:29.600140 django_migration_docs-1.2.0/migration_docs/management/__init__.py
--rw-r--r--   0        0        0        0 2023-11-26 22:45:29.600140 django_migration_docs-1.2.0/migration_docs/management/commands/__init__.py
--rw-r--r--   0        0        0     3975 2023-11-26 22:45:29.600140 django_migration_docs-1.2.0/migration_docs/management/commands/migration_docs.py
--rw-r--r--   0        0        0     4176 2023-11-26 22:45:29.600140 django_migration_docs-1.2.0/migration_docs/utils.py
--rw-r--r--   0        0        0       88 2023-11-26 22:45:29.600140 django_migration_docs-1.2.0/migration_docs/version.py
--rw-r--r--   0        0        0     2350 2023-11-26 22:46:16.632218 django_migration_docs-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 django_migration_docs-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-06 16:12:42.247428 django_migration_docs-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1933 2024-04-06 16:12:42.247428 django_migration_docs-1.2.1/README.md
+-rw-r--r--   0        0        0      419 2024-04-06 16:12:42.251428 django_migration_docs-1.2.1/migration_docs/__init__.py
+-rw-r--r--   0        0        0     1118 2024-04-06 16:12:42.251428 django_migration_docs-1.2.1/migration_docs/apps.py
+-rw-r--r--   0        0        0    16437 2024-04-06 16:12:42.251428 django_migration_docs-1.2.1/migration_docs/core.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:12:42.251428 django_migration_docs-1.2.1/migration_docs/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:12:42.251428 django_migration_docs-1.2.1/migration_docs/management/commands/__init__.py
+-rw-r--r--   0        0        0     3975 2024-04-06 16:12:42.251428 django_migration_docs-1.2.1/migration_docs/management/commands/migration_docs.py
+-rw-r--r--   0        0        0     4176 2024-04-06 16:12:42.255428 django_migration_docs-1.2.1/migration_docs/utils.py
+-rw-r--r--   0        0        0       88 2024-04-06 16:12:42.255428 django_migration_docs-1.2.1/migration_docs/version.py
+-rw-r--r--   0        0        0     2350 2024-04-06 16:13:24.451615 django_migration_docs-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 django_migration_docs-1.2.1/PKG-INFO
```

### Comparing `django_migration_docs-1.2.0/LICENSE` & `django_migration_docs-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_migration_docs-1.2.0/README.md` & `django_migration_docs-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_migration_docs-1.2.0/migration_docs/apps.py` & `django_migration_docs-1.2.1/migration_docs/apps.py`

 * *Files identical despite different names*

### Comparing `django_migration_docs-1.2.0/migration_docs/core.py` & `django_migration_docs-1.2.1/migration_docs/core.py`

 * *Files identical despite different names*

### Comparing `django_migration_docs-1.2.0/migration_docs/management/commands/migration_docs.py` & `django_migration_docs-1.2.1/migration_docs/management/commands/migration_docs.py`

 * *Files identical despite different names*

### Comparing `django_migration_docs-1.2.0/migration_docs/utils.py` & `django_migration_docs-1.2.1/migration_docs/utils.py`

 * *Files identical despite different names*

### Comparing `django_migration_docs-1.2.0/pyproject.toml` & `django_migration_docs-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-migration-docs"
 packages = [
   { include = "migration_docs" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.2.0"
+version = "1.2.1"
 description = "Sync and validate additional information about your Django migrations."
 authors = ["Juliana de Heer", "Wes Kendall", "Tómas Árni Jónasson"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_migration_docs-1.2.0/PKG-INFO` & `django_migration_docs-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-migration-docs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Sync and validate additional information about your Django migrations.
 Home-page: https://github.com/Opus10/django-migration-docs
 License: BSD-3-Clause
 Author: Juliana de Heer
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

