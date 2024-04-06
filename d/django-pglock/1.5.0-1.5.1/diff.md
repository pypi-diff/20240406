# Comparing `tmp/django_pglock-1.5.0.tar.gz` & `tmp/django_pglock-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pglock-1.5.0.tar", max compression
+gzip compressed data, was "django_pglock-1.5.1.tar", max compression
```

## Comparing `django_pglock-1.5.0.tar` & `django_pglock-1.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1456 2023-11-26 22:45:37.399829 django_pglock-1.5.0/LICENSE
--rw-r--r--   0        0        0     4630 2023-11-26 22:45:37.399829 django_pglock-1.5.0/README.md
--rw-r--r--   0        0        0      904 2023-11-26 22:45:37.403829 django_pglock-1.5.0/pglock/__init__.py
--rw-r--r--   0        0        0     1766 2023-11-26 22:45:37.403829 django_pglock-1.5.0/pglock/config.py
--rw-r--r--   0        0        0    20208 2023-11-26 22:45:37.403829 django_pglock-1.5.0/pglock/core.py
--rw-r--r--   0        0        0        0 2023-11-26 22:45:37.403829 django_pglock-1.5.0/pglock/management/__init__.py
--rw-r--r--   0        0        0        0 2023-11-26 22:45:37.403829 django_pglock-1.5.0/pglock/management/commands/__init__.py
--rw-r--r--   0        0        0     5490 2023-11-26 22:45:37.403829 django_pglock-1.5.0/pglock/management/commands/pglock.py
--rw-r--r--   0        0        0     9556 2023-11-26 22:45:37.403829 django_pglock-1.5.0/pglock/models.py
--rw-r--r--   0        0        0      930 2023-11-26 22:45:37.403829 django_pglock-1.5.0/pglock/utils.py
--rw-r--r--   0        0        0       80 2023-11-26 22:45:37.403829 django_pglock-1.5.0/pglock/version.py
--rw-r--r--   0        0        0     2261 2023-11-26 22:46:21.123818 django_pglock-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     5887 1970-01-01 00:00:00.000000 django_pglock-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-06 16:50:16.320116 django_pglock-1.5.1/LICENSE
+-rw-r--r--   0        0        0     4630 2024-04-06 16:50:16.320116 django_pglock-1.5.1/README.md
+-rw-r--r--   0        0        0      904 2024-04-06 16:50:16.320116 django_pglock-1.5.1/pglock/__init__.py
+-rw-r--r--   0        0        0     1766 2024-04-06 16:50:16.320116 django_pglock-1.5.1/pglock/config.py
+-rw-r--r--   0        0        0    20208 2024-04-06 16:50:16.320116 django_pglock-1.5.1/pglock/core.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:50:16.320116 django_pglock-1.5.1/pglock/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:50:16.320116 django_pglock-1.5.1/pglock/management/commands/__init__.py
+-rw-r--r--   0        0        0     5490 2024-04-06 16:50:16.320116 django_pglock-1.5.1/pglock/management/commands/pglock.py
+-rw-r--r--   0        0        0     9556 2024-04-06 16:50:16.320116 django_pglock-1.5.1/pglock/models.py
+-rw-r--r--   0        0        0      930 2024-04-06 16:50:16.320116 django_pglock-1.5.1/pglock/utils.py
+-rw-r--r--   0        0        0       80 2024-04-06 16:50:16.320116 django_pglock-1.5.1/pglock/version.py
+-rw-r--r--   0        0        0     2261 2024-04-06 16:51:06.292086 django_pglock-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5887 1970-01-01 00:00:00.000000 django_pglock-1.5.1/PKG-INFO
```

### Comparing `django_pglock-1.5.0/LICENSE` & `django_pglock-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pglock-1.5.0/README.md` & `django_pglock-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pglock-1.5.0/pglock/__init__.py` & `django_pglock-1.5.1/pglock/__init__.py`

 * *Files identical despite different names*

### Comparing `django_pglock-1.5.0/pglock/config.py` & `django_pglock-1.5.1/pglock/config.py`

 * *Files identical despite different names*

### Comparing `django_pglock-1.5.0/pglock/core.py` & `django_pglock-1.5.1/pglock/core.py`

 * *Files identical despite different names*

### Comparing `django_pglock-1.5.0/pglock/management/commands/pglock.py` & `django_pglock-1.5.1/pglock/management/commands/pglock.py`

 * *Files identical despite different names*

### Comparing `django_pglock-1.5.0/pglock/models.py` & `django_pglock-1.5.1/pglock/models.py`

 * *Files identical despite different names*

### Comparing `django_pglock-1.5.0/pglock/utils.py` & `django_pglock-1.5.1/pglock/utils.py`

 * *Files identical despite different names*

### Comparing `django_pglock-1.5.0/pyproject.toml` & `django_pglock-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pglock"
 packages = [
   { include = "pglock" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.5.0"
+version = "1.5.1"
 description = "Postgres locking routines and lock table access."
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_pglock-1.5.0/PKG-INFO` & `django_pglock-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pglock
-Version: 1.5.0
+Version: 1.5.1
 Summary: Postgres locking routines and lock table access.
 Home-page: https://github.com/Opus10/django-pglock
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

