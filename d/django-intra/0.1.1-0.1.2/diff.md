# Comparing `tmp/django-intra-0.1.1.tar.gz` & `tmp/django-intra-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-intra-0.1.1.tar", last modified: Sat Apr  6 16:50:44 2024, max compression
+gzip compressed data, was "django-intra-0.1.2.tar", last modified: Sat Apr  6 17:28:52 2024, max compression
```

## Comparing `django-intra-0.1.1.tar` & `django-intra-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:44.483005 django-intra-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 16:50:32.000000 django-intra-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-06 16:50:44.483005 django-intra-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-06 16:50:32.000000 django-intra-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:44.483005 django-intra-0.1.1/django_intra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-06 16:50:44.000000 django-intra-0.1.1/django_intra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 16:50:44.000000 django-intra-0.1.1/django_intra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:50:44.000000 django-intra-0.1.1/django_intra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 16:50:44.000000 django-intra-0.1.1/django_intra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 16:50:44.000000 django-intra-0.1.1/django_intra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:44.483005 django-intra-0.1.1/intra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:32.000000 django-intra-0.1.1/intra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-06 16:50:32.000000 django-intra-0.1.1/intra/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 16:50:32.000000 django-intra-0.1.1/intra/intra_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-06 16:50:32.000000 django-intra-0.1.1/intra/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 16:50:32.000000 django-intra-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-06 16:50:44.483005 django-intra-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:50:32.000000 django-intra-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:44.483005 django-intra-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:32.000000 django-intra-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 16:50:32.000000 django-intra-0.1.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-06 16:50:32.000000 django-intra-0.1.1/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-06 16:50:32.000000 django-intra-0.1.1/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:28:52.065340 django-intra-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 17:28:43.000000 django-intra-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-06 17:28:52.065340 django-intra-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-06 17:28:43.000000 django-intra-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:28:52.065340 django-intra-0.1.2/django_intra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-06 17:28:52.000000 django-intra-0.1.2/django_intra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 17:28:52.000000 django-intra-0.1.2/django_intra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:28:52.000000 django-intra-0.1.2/django_intra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 17:28:52.000000 django-intra-0.1.2/django_intra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 17:28:52.000000 django-intra-0.1.2/django_intra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:28:52.061340 django-intra-0.1.2/intra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:28:43.000000 django-intra-0.1.2/intra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-06 17:28:43.000000 django-intra-0.1.2/intra/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 17:28:43.000000 django-intra-0.1.2/intra/intra_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-06 17:28:43.000000 django-intra-0.1.2/intra/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 17:28:43.000000 django-intra-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-06 17:28:52.065340 django-intra-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 17:28:43.000000 django-intra-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:28:52.065340 django-intra-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:28:43.000000 django-intra-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 17:28:43.000000 django-intra-0.1.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-06 17:28:43.000000 django-intra-0.1.2/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-06 17:28:43.000000 django-intra-0.1.2/tests/urls.py
```

### Comparing `django-intra-0.1.1/LICENSE` & `django-intra-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.1/PKG-INFO` & `django-intra-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-intra
-Version: 0.1.1
+Version: 0.1.2
 Summary: An extension of the Django admin application with special features
 Home-page: https://github.com/ahmdhjj/django-intra
 Author: ahmdhjj
 Author-email: ahmdhjj@example.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-intra-0.1.1/README.md` & `django-intra-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.1/django_intra.egg-info/PKG-INFO` & `django-intra-0.1.2/django_intra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-intra
-Version: 0.1.1
+Version: 0.1.2
 Summary: An extension of the Django admin application with special features
 Home-page: https://github.com/ahmdhjj/django-intra
 Author: ahmdhjj
 Author-email: ahmdhjj@example.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-intra-0.1.1/intra/urls.py` & `django-intra-0.1.2/intra/urls.py`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.1/setup.cfg` & `django-intra-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-intra
-version = 0.1.1
+version = 0.1.2
 description = An extension of the Django admin application with special features
 long_description = An extension of the Django admin application with special features
 url = https://github.com/ahmdhjj/django-intra
 author = ahmdhjj
 author_email = ahmdhjj@example.com
 license = MIT License
 classifiers =
```

### Comparing `django-intra-0.1.1/tests/settings.py` & `django-intra-0.1.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.1/tests/tests.py` & `django-intra-0.1.2/tests/tests.py`

 * *Files identical despite different names*

