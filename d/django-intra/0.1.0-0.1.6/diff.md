# Comparing `tmp/django-intra-0.1.0.tar.gz` & `tmp/django-intra-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-intra-0.1.0.tar", last modified: Thu Apr  4 22:28:20 2024, max compression
+gzip compressed data, was "django-intra-0.1.6.tar", last modified: Sat Apr  6 19:01:31 2024, max compression
```

## Comparing `django-intra-0.1.0.tar` & `django-intra-0.1.6.tar`

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
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:31.339573 django-intra-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 19:01:26.000000 django-intra-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-06 19:01:31.339573 django-intra-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-06 19:01:26.000000 django-intra-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:31.339573 django-intra-0.1.6/django_intra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-06 19:01:31.000000 django-intra-0.1.6/django_intra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 19:01:31.000000 django-intra-0.1.6/django_intra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:01:31.000000 django-intra-0.1.6/django_intra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 19:01:31.000000 django-intra-0.1.6/django_intra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 19:01:31.000000 django-intra-0.1.6/django_intra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:31.339573 django-intra-0.1.6/intra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:26.000000 django-intra-0.1.6/intra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-06 19:01:26.000000 django-intra-0.1.6/intra/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 19:01:26.000000 django-intra-0.1.6/intra/intra_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-06 19:01:26.000000 django-intra-0.1.6/intra/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 19:01:26.000000 django-intra-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-06 19:01:31.339573 django-intra-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:01:26.000000 django-intra-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:31.339573 django-intra-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:26.000000 django-intra-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 19:01:26.000000 django-intra-0.1.6/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-06 19:01:26.000000 django-intra-0.1.6/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-06 19:01:26.000000 django-intra-0.1.6/tests/urls.py
```

### Comparing `django-intra-0.1.0/LICENSE` & `django-intra-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.0/README.md` & `django-intra-0.1.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+[![PyPI](https://img.shields.io/pypi/v/django-intra)](https://pypi.org/project/django-intra/)
+
 [![Pylint](https://github.com/ahmdhjj/django-intra/actions/workflows/pylint.yml/badge.svg)](https://github.com/ahmdhjj/django-intra/actions/workflows/pylint.yml)
 [![Django CI](https://github.com/ahmdhjj/django-intra/actions/workflows/test.yml/badge.svg)](https://github.com/ahmdhjj/django-intra/actions/workflows/test.yml)
+[![Upload Python Package](https://github.com/ahmdhjj/django-intra/actions/workflows/release.yml/badge.svg)](https://github.com/ahmdhjj/django-intra/actions/workflows/release.yml)
 # django-intra
+## Installation
+```
+pip install django-intra
+```
 ## Settings
 In your settings file:
 1. Add `'intra'` to `INSTALLED_APPS`.
-3. Add `'intra/templates'` to the `DIRS` option in the `TEMPLATES` setting.
+
+2. Add `'intra/templates'` to the `DIRS` option in the `TEMPLATES` setting:
 ```
   TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': ['intra/templates'],
         'APP_DIRS': True,
         'OPTIONS': {
```

### Comparing `django-intra-0.1.0/intra/urls.py` & `django-intra-0.1.6/intra/urls.py`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.0/tests/settings.py` & `django-intra-0.1.6/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.0/tests/tests.py` & `django-intra-0.1.6/tests/tests.py`

 * *Files identical despite different names*

