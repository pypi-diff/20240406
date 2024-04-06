# Comparing `tmp/django_pgactivity-1.4.0.tar.gz` & `tmp/django_pgactivity-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgactivity-1.4.0.tar", max compression
+gzip compressed data, was "django_pgactivity-1.4.1.tar", max compression
```

## Comparing `django_pgactivity-1.4.0.tar` & `django_pgactivity-1.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1456 2023-11-26 22:45:30.471187 django_pgactivity-1.4.0/LICENSE
--rw-r--r--   0        0        0     3931 2023-11-26 22:45:30.471187 django_pgactivity-1.4.0/README.md
--rw-r--r--   0        0        0      266 2023-11-26 22:45:30.471187 django_pgactivity-1.4.0/pgactivity/__init__.py
--rw-r--r--   0        0        0     1641 2023-11-26 22:45:30.471187 django_pgactivity-1.4.0/pgactivity/config.py
--rw-r--r--   0        0        0     1349 2023-11-26 22:45:30.471187 django_pgactivity-1.4.0/pgactivity/contrib.py
--rw-r--r--   0        0        0     5040 2023-11-26 22:45:30.471187 django_pgactivity-1.4.0/pgactivity/core.py
--rw-r--r--   0        0        0        0 2023-11-26 22:45:30.471187 django_pgactivity-1.4.0/pgactivity/management/__init__.py
--rw-r--r--   0        0        0        0 2023-11-26 22:45:30.471187 django_pgactivity-1.4.0/pgactivity/management/commands/__init__.py
--rw-r--r--   0        0        0     4305 2023-11-26 22:45:30.475187 django_pgactivity-1.4.0/pgactivity/management/commands/pgactivity.py
--rw-r--r--   0        0        0      347 2023-11-26 22:45:30.475187 django_pgactivity-1.4.0/pgactivity/middleware.py
--rw-r--r--   0        0        0     8656 2023-11-26 22:45:30.475187 django_pgactivity-1.4.0/pgactivity/models.py
--rw-r--r--   0        0        0     2343 2023-11-26 22:45:30.475187 django_pgactivity-1.4.0/pgactivity/runtime.py
--rw-r--r--   0        0        0     1099 2023-11-26 22:45:30.475187 django_pgactivity-1.4.0/pgactivity/utils.py
--rw-r--r--   0        0        0       84 2023-11-26 22:45:30.475187 django_pgactivity-1.4.0/pgactivity/version.py
--rw-r--r--   0        0        0     2253 2023-11-26 22:46:14.367206 django_pgactivity-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 django_pgactivity-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/LICENSE
+-rw-r--r--   0        0        0     3931 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/README.md
+-rw-r--r--   0        0        0      266 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/__init__.py
+-rw-r--r--   0        0        0     1641 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/config.py
+-rw-r--r--   0        0        0     1349 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/contrib.py
+-rw-r--r--   0        0        0     5040 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/core.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/management/commands/__init__.py
+-rw-r--r--   0        0        0     4305 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/management/commands/pgactivity.py
+-rw-r--r--   0        0        0      347 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/middleware.py
+-rw-r--r--   0        0        0     8656 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/models.py
+-rw-r--r--   0        0        0     2343 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/runtime.py
+-rw-r--r--   0        0        0     1099 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/utils.py
+-rw-r--r--   0        0        0       84 2024-04-06 16:50:15.030651 django_pgactivity-1.4.1/pgactivity/version.py
+-rw-r--r--   0        0        0     2253 2024-04-06 16:51:00.090876 django_pgactivity-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 django_pgactivity-1.4.1/PKG-INFO
```

### Comparing `django_pgactivity-1.4.0/LICENSE` & `django_pgactivity-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgactivity-1.4.0/README.md` & `django_pgactivity-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pgactivity-1.4.0/pgactivity/config.py` & `django_pgactivity-1.4.1/pgactivity/config.py`

 * *Files identical despite different names*

### Comparing `django_pgactivity-1.4.0/pgactivity/contrib.py` & `django_pgactivity-1.4.1/pgactivity/contrib.py`

 * *Files identical despite different names*

### Comparing `django_pgactivity-1.4.0/pgactivity/core.py` & `django_pgactivity-1.4.1/pgactivity/core.py`

 * *Files identical despite different names*

### Comparing `django_pgactivity-1.4.0/pgactivity/management/commands/pgactivity.py` & `django_pgactivity-1.4.1/pgactivity/management/commands/pgactivity.py`

 * *Files identical despite different names*

### Comparing `django_pgactivity-1.4.0/pgactivity/models.py` & `django_pgactivity-1.4.1/pgactivity/models.py`

 * *Files identical despite different names*

### Comparing `django_pgactivity-1.4.0/pgactivity/runtime.py` & `django_pgactivity-1.4.1/pgactivity/runtime.py`

 * *Files identical despite different names*

### Comparing `django_pgactivity-1.4.0/pgactivity/utils.py` & `django_pgactivity-1.4.1/pgactivity/utils.py`

 * *Files identical despite different names*

### Comparing `django_pgactivity-1.4.0/pyproject.toml` & `django_pgactivity-1.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pgactivity"
 packages = [
   { include = "pgactivity" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.4.0"
+version = "1.4.1"
 description = "Monitor, kill, and analyze Postgres queries."
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_pgactivity-1.4.0/PKG-INFO` & `django_pgactivity-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgactivity
-Version: 1.4.0
+Version: 1.4.1
 Summary: Monitor, kill, and analyze Postgres queries.
 Home-page: https://github.com/Opus10/django-pgactivity
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

