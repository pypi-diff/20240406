# Comparing `tmp/django_layui29-0.1.0.tar.gz` & `tmp/django_layui29-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_layui29-0.1.0.tar", max compression
+gzip compressed data, was "django_layui29-0.1.1.tar", max compression
```

## Comparing `django_layui29-0.1.0.tar` & `django_layui29-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1270 2024-04-06 05:01:05.929798 django_layui29-0.1.0/LICENSE
--rw-r--r--   0        0        0      950 2024-04-06 05:04:50.987349 django_layui29-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-06 04:54:09.874487 django_layui29-0.1.0/src/django_layui29/__init__.py
--rw-r--r--   0        0        0       66 2024-04-06 04:54:09.875486 django_layui29-0.1.0/src/django_layui29/admin.py
--rw-r--r--   0        0        0      161 2024-04-06 04:54:09.875486 django_layui29-0.1.0/src/django_layui29/apps.py
--rw-r--r--   0        0        0        0 2024-04-06 04:54:09.875486 django_layui29-0.1.0/src/django_layui29/migrations/__init__.py
--rw-r--r--   0        0        0       60 2024-04-06 04:54:09.875486 django_layui29-0.1.0/src/django_layui29/models.py
--rw-r--r--   0        0        0      556 2024-04-06 04:57:22.665192 django_layui29-0.1.0/src/django_layui29/templates/layui29/base.html
--rw-r--r--   0        0        0       63 2024-04-06 04:54:09.876486 django_layui29-0.1.0/src/django_layui29/tests.py
--rw-r--r--   0        0        0       66 2024-04-06 04:54:09.876486 django_layui29-0.1.0/src/django_layui29/views.py
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 django_layui29-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1270 2024-04-06 05:01:05.929798 django_layui29-0.1.1/LICENSE
+-rw-r--r--   0        0        0      950 2024-04-06 05:13:14.530490 django_layui29-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-06 04:54:09.874487 django_layui29-0.1.1/src/django_layui29/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-06 04:54:09.875486 django_layui29-0.1.1/src/django_layui29/admin.py
+-rw-r--r--   0        0        0      163 2024-04-06 05:13:09.757522 django_layui29-0.1.1/src/django_layui29/apps.py
+-rw-r--r--   0        0        0        0 2024-04-06 04:54:09.875486 django_layui29-0.1.1/src/django_layui29/migrations/__init__.py
+-rw-r--r--   0        0        0       60 2024-04-06 04:54:09.875486 django_layui29-0.1.1/src/django_layui29/models.py
+-rw-r--r--   0        0        0      556 2024-04-06 04:57:22.665192 django_layui29-0.1.1/src/django_layui29/templates/layui29/base.html
+-rw-r--r--   0        0        0       63 2024-04-06 04:54:09.876486 django_layui29-0.1.1/src/django_layui29/tests.py
+-rw-r--r--   0        0        0       66 2024-04-06 04:54:09.876486 django_layui29-0.1.1/src/django_layui29/views.py
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 django_layui29-0.1.1/PKG-INFO
```

### Comparing `django_layui29-0.1.0/LICENSE` & `django_layui29-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_layui29-0.1.0/pyproject.toml` & `django_layui29-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django_layui29"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["svtter <svtter@163.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 django = "<6.0"
```

### Comparing `django_layui29-0.1.0/src/django_layui29/templates/layui29/base.html` & `django_layui29-0.1.1/src/django_layui29/templates/layui29/base.html`

 * *Files identical despite different names*

### Comparing `django_layui29-0.1.0/PKG-INFO` & `django_layui29-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_layui29
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: svtter
 Author-email: svtter@163.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

