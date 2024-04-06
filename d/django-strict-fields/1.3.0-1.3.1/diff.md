# Comparing `tmp/django_strict_fields-1.3.0.tar.gz` & `tmp/django_strict_fields-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_strict_fields-1.3.0.tar", max compression
+gzip compressed data, was "django_strict_fields-1.3.1.tar", max compression
```

## Comparing `django_strict_fields-1.3.0.tar` & `django_strict_fields-1.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1456 2023-11-26 22:56:59.479515 django_strict_fields-1.3.0/LICENSE
--rw-r--r--   0        0        0      829 2023-11-26 22:56:59.479515 django_strict_fields-1.3.0/README.md
--rw-r--r--   0        0        0     2251 2023-11-26 22:57:44.783638 django_strict_fields-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      442 2023-11-26 22:56:59.483516 django_strict_fields-1.3.0/strict_fields/__init__.py
--rw-r--r--   0        0        0     3032 2023-11-26 22:56:59.483516 django_strict_fields-1.3.0/strict_fields/apps.py
--rw-r--r--   0        0        0     2900 2023-11-26 22:56:59.483516 django_strict_fields-1.3.0/strict_fields/fields.py
--rw-r--r--   0        0        0      990 2023-11-26 22:56:59.483516 django_strict_fields-1.3.0/strict_fields/helpers.py
--rw-r--r--   0        0        0       87 2023-11-26 22:56:59.483516 django_strict_fields-1.3.0/strict_fields/version.py
--rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 django_strict_fields-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-06 16:49:42.202648 django_strict_fields-1.3.1/LICENSE
+-rw-r--r--   0        0        0      829 2024-04-06 16:49:42.202648 django_strict_fields-1.3.1/README.md
+-rw-r--r--   0        0        0     2251 2024-04-06 16:50:25.818954 django_strict_fields-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      442 2024-04-06 16:49:42.206648 django_strict_fields-1.3.1/strict_fields/__init__.py
+-rw-r--r--   0        0        0     3032 2024-04-06 16:49:42.206648 django_strict_fields-1.3.1/strict_fields/apps.py
+-rw-r--r--   0        0        0     2900 2024-04-06 16:49:42.206648 django_strict_fields-1.3.1/strict_fields/fields.py
+-rw-r--r--   0        0        0      990 2024-04-06 16:49:42.206648 django_strict_fields-1.3.1/strict_fields/helpers.py
+-rw-r--r--   0        0        0       87 2024-04-06 16:49:42.206648 django_strict_fields-1.3.1/strict_fields/version.py
+-rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 django_strict_fields-1.3.1/PKG-INFO
```

### Comparing `django_strict_fields-1.3.0/LICENSE` & `django_strict_fields-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.0/README.md` & `django_strict_fields-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.0/pyproject.toml` & `django_strict_fields-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-strict-fields"
 packages = [
   { include = "strict_fields" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.3.0"
+version = "1.3.1"
 description = "A collection of fields and utilities to help make model fields more strict."
 authors = ["Tomas Arni Jonasson"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_strict_fields-1.3.0/strict_fields/apps.py` & `django_strict_fields-1.3.1/strict_fields/apps.py`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.0/strict_fields/fields.py` & `django_strict_fields-1.3.1/strict_fields/fields.py`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.0/strict_fields/helpers.py` & `django_strict_fields-1.3.1/strict_fields/helpers.py`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.0/PKG-INFO` & `django_strict_fields-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-strict-fields
-Version: 1.3.0
+Version: 1.3.1
 Summary: A collection of fields and utilities to help make model fields more strict.
 Home-page: https://github.com/Opus10/django-strict-fields
 License: BSD-3-Clause
 Author: Tomas Arni Jonasson
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

