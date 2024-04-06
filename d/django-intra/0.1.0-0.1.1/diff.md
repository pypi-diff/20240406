# Comparing `tmp/django-intra-0.1.0.tar.gz` & `tmp/django-intra-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-intra-0.1.0.tar", last modified: Thu Apr  4 22:28:20 2024, max compression
+gzip compressed data, was "django-intra-0.1.1.tar", last modified: Sat Apr  6 16:50:44 2024, max compression
```

## Comparing `django-intra-0.1.0.tar` & `django-intra-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:20.300956 django-intra-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 22:28:14.000000 django-intra-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-04 22:28:20.300956 django-intra-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-04 22:28:14.000000 django-intra-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:20.300956 django-intra-0.1.0/django_intra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-04 22:28:20.000000 django-intra-0.1.0/django_intra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-04 22:28:20.000000 django-intra-0.1.0/django_intra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:28:20.000000 django-intra-0.1.0/django_intra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 22:28:20.000000 django-intra-0.1.0/django_intra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 22:28:20.000000 django-intra-0.1.0/django_intra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:20.300956 django-intra-0.1.0/intra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:14.000000 django-intra-0.1.0/intra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 22:28:14.000000 django-intra-0.1.0/intra/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-04 22:28:14.000000 django-intra-0.1.0/intra/intra_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 22:28:14.000000 django-intra-0.1.0/intra/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 22:28:14.000000 django-intra-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-04 22:28:20.304956 django-intra-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:28:14.000000 django-intra-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:20.300956 django-intra-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:14.000000 django-intra-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 22:28:14.000000 django-intra-0.1.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-04 22:28:14.000000 django-intra-0.1.0/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-04 22:28:14.000000 django-intra-0.1.0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:44.483005 django-intra-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 16:50:32.000000 django-intra-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-06 16:50:44.483005 django-intra-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-06 16:50:32.000000 django-intra-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:44.483005 django-intra-0.1.1/django_intra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-06 16:50:44.000000 django-intra-0.1.1/django_intra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 16:50:44.000000 django-intra-0.1.1/django_intra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:50:44.000000 django-intra-0.1.1/django_intra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 16:50:44.000000 django-intra-0.1.1/django_intra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 16:50:44.000000 django-intra-0.1.1/django_intra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:44.483005 django-intra-0.1.1/intra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:32.000000 django-intra-0.1.1/intra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-06 16:50:32.000000 django-intra-0.1.1/intra/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 16:50:32.000000 django-intra-0.1.1/intra/intra_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-06 16:50:32.000000 django-intra-0.1.1/intra/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 16:50:32.000000 django-intra-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-06 16:50:44.483005 django-intra-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:50:32.000000 django-intra-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:44.483005 django-intra-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:32.000000 django-intra-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 16:50:32.000000 django-intra-0.1.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-06 16:50:32.000000 django-intra-0.1.1/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-06 16:50:32.000000 django-intra-0.1.1/tests/urls.py
```

### Comparing `django-intra-0.1.0/LICENSE` & `django-intra-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.0/PKG-INFO` & `django-intra-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-intra
-Version: 0.1.0
+Version: 0.1.1
 Summary: An extension of the Django admin application with special features
 Home-page: https://github.com/ahmdhjj/django-intra
 Author: ahmdhjj
 Author-email: ahmdhjj@example.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-intra-0.1.0/README.md` & `django-intra-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [![Pylint](https://github.com/ahmdhjj/django-intra/actions/workflows/pylint.yml/badge.svg)](https://github.com/ahmdhjj/django-intra/actions/workflows/pylint.yml)
 [![Django CI](https://github.com/ahmdhjj/django-intra/actions/workflows/test.yml/badge.svg)](https://github.com/ahmdhjj/django-intra/actions/workflows/test.yml)
+[![Upload Python Package](https://github.com/ahmdhjj/django-intra/actions/workflows/release.yml/badge.svg)](https://github.com/ahmdhjj/django-intra/actions/workflows/release.yml)
 # django-intra
 ## Settings
 In your settings file:
 1. Add `'intra'` to `INSTALLED_APPS`.
 3. Add `'intra/templates'` to the `DIRS` option in the `TEMPLATES` setting.
 ```
   TEMPLATES = [
```

### Comparing `django-intra-0.1.0/django_intra.egg-info/PKG-INFO` & `django-intra-0.1.1/django_intra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-intra
-Version: 0.1.0
+Version: 0.1.1
 Summary: An extension of the Django admin application with special features
 Home-page: https://github.com/ahmdhjj/django-intra
 Author: ahmdhjj
 Author-email: ahmdhjj@example.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-intra-0.1.0/intra/urls.py` & `django-intra-0.1.1/intra/urls.py`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.0/setup.cfg` & `django-intra-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-intra
-version = 0.1.0
+version = 0.1.1
 description = An extension of the Django admin application with special features
 long_description = An extension of the Django admin application with special features
 url = https://github.com/ahmdhjj/django-intra
 author = ahmdhjj
 author_email = ahmdhjj@example.com
 license = MIT License
 classifiers =
```

### Comparing `django-intra-0.1.0/tests/settings.py` & `django-intra-0.1.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.0/tests/tests.py` & `django-intra-0.1.1/tests/tests.py`

 * *Files identical despite different names*

