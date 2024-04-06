# Comparing `tmp/django_pgtransaction-1.3.0.tar.gz` & `tmp/django_pgtransaction-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgtransaction-1.3.0.tar", max compression
+gzip compressed data, was "django_pgtransaction-1.3.1.tar", max compression
```

## Comparing `django_pgtransaction-1.3.0.tar` & `django_pgtransaction-1.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1456 2023-11-26 22:57:11.079887 django_pgtransaction-1.3.0/LICENSE
--rw-r--r--   0        0        0     3038 2023-11-26 22:57:11.079887 django_pgtransaction-1.3.0/README.md
--rw-r--r--   0        0        0      224 2023-11-26 22:57:11.083888 django_pgtransaction-1.3.0/pgtransaction/__init__.py
--rw-r--r--   0        0        0      731 2023-11-26 22:57:11.083888 django_pgtransaction-1.3.0/pgtransaction/config.py
--rw-r--r--   0        0        0     7377 2023-11-26 22:57:11.083888 django_pgtransaction-1.3.0/pgtransaction/transaction.py
--rw-r--r--   0        0        0       87 2023-11-26 22:57:11.083888 django_pgtransaction-1.3.0/pgtransaction/version.py
--rw-r--r--   0        0        0     2297 2023-11-26 22:57:51.811611 django_pgtransaction-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 django_pgtransaction-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-06 16:50:31.417333 django_pgtransaction-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3038 2024-04-06 16:50:31.421333 django_pgtransaction-1.3.1/README.md
+-rw-r--r--   0        0        0      224 2024-04-06 16:50:31.421333 django_pgtransaction-1.3.1/pgtransaction/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-06 16:50:31.421333 django_pgtransaction-1.3.1/pgtransaction/config.py
+-rw-r--r--   0        0        0     7377 2024-04-06 16:50:31.421333 django_pgtransaction-1.3.1/pgtransaction/transaction.py
+-rw-r--r--   0        0        0       87 2024-04-06 16:50:31.421333 django_pgtransaction-1.3.1/pgtransaction/version.py
+-rw-r--r--   0        0        0     2297 2024-04-06 16:51:16.085864 django_pgtransaction-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 django_pgtransaction-1.3.1/PKG-INFO
```

### Comparing `django_pgtransaction-1.3.0/LICENSE` & `django_pgtransaction-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgtransaction-1.3.0/README.md` & `django_pgtransaction-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pgtransaction-1.3.0/pgtransaction/config.py` & `django_pgtransaction-1.3.1/pgtransaction/config.py`

 * *Files identical despite different names*

### Comparing `django_pgtransaction-1.3.0/pgtransaction/transaction.py` & `django_pgtransaction-1.3.1/pgtransaction/transaction.py`

 * *Files identical despite different names*

### Comparing `django_pgtransaction-1.3.0/pyproject.toml` & `django_pgtransaction-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pgtransaction"
 packages = [
   { include = "pgtransaction" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.3.0"
+version = "1.3.1"
 description = "A context manager/decorator which extends Django's atomic function with the ability to set isolation level and retries for a given transaction."
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_pgtransaction-1.3.0/PKG-INFO` & `django_pgtransaction-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgtransaction
-Version: 1.3.0
+Version: 1.3.1
 Summary: A context manager/decorator which extends Django's atomic function with the ability to set isolation level and retries for a given transaction.
 Home-page: https://github.com/Opus10/django-pgtransaction
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

