# Comparing `tmp/django_pgbulk-2.3.0.tar.gz` & `tmp/django_pgbulk-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgbulk-2.3.0.tar", max compression
+gzip compressed data, was "django_pgbulk-2.3.1.tar", max compression
```

## Comparing `django_pgbulk-2.3.0.tar` & `django_pgbulk-2.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1456 2023-12-27 22:34:25.615866 django_pgbulk-2.3.0/LICENSE
--rw-r--r--   0        0        0     2051 2023-12-27 22:34:25.615866 django_pgbulk-2.3.0/README.md
--rw-r--r--   0        0        0      920 2023-12-27 22:34:25.615866 django_pgbulk-2.3.0/pgbulk/__init__.py
--rw-r--r--   0        0        0    23943 2023-12-27 22:34:25.615866 django_pgbulk-2.3.0/pgbulk/core.py
--rw-r--r--   0        0        0        0 2023-12-27 22:34:25.615866 django_pgbulk-2.3.0/pgbulk/py.typed
--rw-r--r--   0        0        0       80 2023-12-27 22:34:25.615866 django_pgbulk-2.3.0/pgbulk/version.py
--rw-r--r--   0        0        0     2198 2023-12-27 22:35:13.415923 django_pgbulk-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 django_pgbulk-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/LICENSE
+-rw-r--r--   0        0        0     2051 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/README.md
+-rw-r--r--   0        0        0      920 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/pgbulk/__init__.py
+-rw-r--r--   0        0        0    23943 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/pgbulk/core.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/pgbulk/py.typed
+-rw-r--r--   0        0        0       80 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/pgbulk/version.py
+-rw-r--r--   0        0        0     2198 2024-04-06 16:50:24.110373 django_pgbulk-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 django_pgbulk-2.3.1/PKG-INFO
```

### Comparing `django_pgbulk-2.3.0/LICENSE` & `django_pgbulk-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgbulk-2.3.0/README.md` & `django_pgbulk-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pgbulk-2.3.0/pgbulk/__init__.py` & `django_pgbulk-2.3.1/pgbulk/__init__.py`

 * *Files identical despite different names*

### Comparing `django_pgbulk-2.3.0/pgbulk/core.py` & `django_pgbulk-2.3.1/pgbulk/core.py`

 * *Files identical despite different names*

### Comparing `django_pgbulk-2.3.0/pyproject.toml` & `django_pgbulk-2.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pgbulk"
 packages = [
   { include = "pgbulk" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "2.3.0"
+version = "2.3.1"
 description = "Native postgres bulk update and upsert operations."
 authors = ["Wes Kendall"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_pgbulk-2.3.0/PKG-INFO` & `django_pgbulk-2.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgbulk
-Version: 2.3.0
+Version: 2.3.1
 Summary: Native postgres bulk update and upsert operations.
 Home-page: https://github.com/Opus10/django-pgbulk
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

