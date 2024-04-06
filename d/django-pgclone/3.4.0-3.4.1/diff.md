# Comparing `tmp/django_pgclone-3.4.0.tar.gz` & `tmp/django_pgclone-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgclone-3.4.0.tar", max compression
+gzip compressed data, was "django_pgclone-3.4.1.tar", max compression
```

## Comparing `django_pgclone-3.4.0.tar` & `django_pgclone-3.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1456 2023-12-06 00:51:34.913583 django_pgclone-3.4.0/LICENSE
--rw-r--r--   0        0        0     2395 2023-12-06 00:51:34.913583 django_pgclone-3.4.0/README.md
--rw-r--r--   0        0        0      238 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/__init__.py
--rw-r--r--   0        0        0     2166 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/copy_cmd.py
--rw-r--r--   0        0        0     6241 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/db.py
--rw-r--r--   0        0        0     3481 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/dump_cmd.py
--rw-r--r--   0        0        0      438 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/exceptions.py
--rw-r--r--   0        0        0     2169 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/logging.py
--rw-r--r--   0        0        0     3439 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/ls_cmd.py
--rw-r--r--   0        0        0        0 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/management/commands/__init__.py
--rw-r--r--   0        0        0     7201 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/management/commands/pgclone.py
--rw-r--r--   0        0        0     2483 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/options.py
--rw-r--r--   0        0        0     9399 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/restore_cmd.py
--rw-r--r--   0        0        0     1604 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/run.py
--rw-r--r--   0        0        0     2220 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/settings.py
--rw-r--r--   0        0        0     3505 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/storage.py
--rw-r--r--   0        0        0       81 2023-12-06 00:51:34.917583 django_pgclone-3.4.0/pgclone/version.py
--rw-r--r--   0        0        0     2212 2023-12-06 00:52:26.477922 django_pgclone-3.4.0/pyproject.toml
--rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 django_pgclone-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/LICENSE
+-rw-r--r--   0        0        0     2395 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/README.md
+-rw-r--r--   0        0        0      238 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/__init__.py
+-rw-r--r--   0        0        0     2166 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/copy_cmd.py
+-rw-r--r--   0        0        0     6241 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/db.py
+-rw-r--r--   0        0        0     3481 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/dump_cmd.py
+-rw-r--r--   0        0        0      438 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/exceptions.py
+-rw-r--r--   0        0        0     2169 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/logging.py
+-rw-r--r--   0        0        0     3439 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/ls_cmd.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/management/commands/__init__.py
+-rw-r--r--   0        0        0     7201 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/management/commands/pgclone.py
+-rw-r--r--   0        0        0     2483 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/options.py
+-rw-r--r--   0        0        0     9399 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/restore_cmd.py
+-rw-r--r--   0        0        0     1604 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/run.py
+-rw-r--r--   0        0        0     2220 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/settings.py
+-rw-r--r--   0        0        0     3505 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/storage.py
+-rw-r--r--   0        0        0       81 2024-04-06 16:50:46.804562 django_pgclone-3.4.1/pgclone/version.py
+-rw-r--r--   0        0        0     2212 2024-04-06 16:51:33.656624 django_pgclone-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 django_pgclone-3.4.1/PKG-INFO
```

### Comparing `django_pgclone-3.4.0/LICENSE` & `django_pgclone-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/README.md` & `django_pgclone-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/copy_cmd.py` & `django_pgclone-3.4.1/pgclone/copy_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/db.py` & `django_pgclone-3.4.1/pgclone/db.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/dump_cmd.py` & `django_pgclone-3.4.1/pgclone/dump_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/logging.py` & `django_pgclone-3.4.1/pgclone/logging.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/ls_cmd.py` & `django_pgclone-3.4.1/pgclone/ls_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/management/commands/pgclone.py` & `django_pgclone-3.4.1/pgclone/management/commands/pgclone.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/options.py` & `django_pgclone-3.4.1/pgclone/options.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/restore_cmd.py` & `django_pgclone-3.4.1/pgclone/restore_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/run.py` & `django_pgclone-3.4.1/pgclone/run.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/settings.py` & `django_pgclone-3.4.1/pgclone/settings.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pgclone/storage.py` & `django_pgclone-3.4.1/pgclone/storage.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.4.0/pyproject.toml` & `django_pgclone-3.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pgclone"
 packages = [
   { include = "pgclone" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "3.4.0"
+version = "3.4.1"
 description = "Dump and restore Postgres databases with Django."
 authors = ["Wes Kendall", "Ethan O'Brien"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_pgclone-3.4.0/PKG-INFO` & `django_pgclone-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgclone
-Version: 3.4.0
+Version: 3.4.1
 Summary: Dump and restore Postgres databases with Django.
 Home-page: https://github.com/Opus10/django-pgclone
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

