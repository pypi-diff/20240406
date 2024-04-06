# Comparing `tmp/django-rahavard-0.0.16.tar.gz` & `tmp/django-rahavard-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rahavard-0.0.16.tar", last modified: Thu Mar 28 20:06:16 2024, max compression
+gzip compressed data, was "django-rahavard-0.0.17.tar", last modified: Sat Apr  6 03:04:59 2024, max compression
```

## Comparing `django-rahavard-0.0.16.tar` & `django-rahavard-0.0.17.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-28 20:06:16.900889 django-rahavard-0.0.16/
--rw-r--r--   0 nino      (1000) nino      (1000)     1072 2024-03-22 09:57:46.000000 django-rahavard-0.0.16/LICENSE
--rw-r--r--   0 nino      (1000) nino      (1000)      897 2024-03-28 20:06:16.900889 django-rahavard-0.0.16/PKG-INFO
--rw-r--r--   0 nino      (1000) nino      (1000)      100 2024-03-22 12:38:40.000000 django-rahavard-0.0.16/README.md
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-28 20:06:16.894222 django-rahavard-0.0.16/django_rahavard/
--rw-r--r--   0 nino      (1000) nino      (1000)        0 2024-03-22 08:57:54.000000 django-rahavard-0.0.16/django_rahavard/__init__.py
--rw-r--r--   0 nino      (1000) nino      (1000)      191 2024-03-22 09:50:24.000000 django-rahavard-0.0.16/django_rahavard/apps.py
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-28 20:06:16.897555 django-rahavard-0.0.16/django_rahavard/management/
--rw-r--r--   0 nino      (1000) nino      (1000)        0 2024-03-22 08:57:54.000000 django-rahavard-0.0.16/django_rahavard/management/__init__.py
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-28 20:06:16.897555 django-rahavard-0.0.16/django_rahavard/management/commands/
--rw-r--r--   0 nino      (1000) nino      (1000)        0 2024-03-22 08:57:54.000000 django-rahavard-0.0.16/django_rahavard/management/commands/__init__.py
--rw-r--r--   0 nino      (1000) nino      (1000)      650 2024-03-22 08:57:54.000000 django-rahavard-0.0.16/django_rahavard/management/commands/check_deploy.py
--rw-r--r--   0 nino      (1000) nino      (1000)     1923 2024-03-22 08:57:54.000000 django-rahavard-0.0.16/django_rahavard/management/commands/collectstatic.py
--rw-r--r--   0 nino      (1000) nino      (1000)     2838 2024-03-28 19:56:45.000000 django-rahavard-0.0.16/django_rahavard/management/commands/dumpdata.py
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-28 20:06:16.897555 django-rahavard-0.0.16/django_rahavard/migrations/
--rw-r--r--   0 nino      (1000) nino      (1000)        0 2024-03-22 08:57:54.000000 django-rahavard-0.0.16/django_rahavard/migrations/__init__.py
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-28 20:06:16.897555 django-rahavard-0.0.16/django_rahavard.egg-info/
--rw-r--r--   0 nino      (1000) nino      (1000)      897 2024-03-28 20:06:16.000000 django-rahavard-0.0.16/django_rahavard.egg-info/PKG-INFO
--rw-r--r--   0 nino      (1000) nino      (1000)      576 2024-03-28 20:06:16.000000 django-rahavard-0.0.16/django_rahavard.egg-info/SOURCES.txt
--rw-r--r--   0 nino      (1000) nino      (1000)        1 2024-03-28 20:06:16.000000 django-rahavard-0.0.16/django_rahavard.egg-info/dependency_links.txt
--rw-r--r--   0 nino      (1000) nino      (1000)       16 2024-03-28 20:06:16.000000 django-rahavard-0.0.16/django_rahavard.egg-info/requires.txt
--rw-r--r--   0 nino      (1000) nino      (1000)       16 2024-03-28 20:06:16.000000 django-rahavard-0.0.16/django_rahavard.egg-info/top_level.txt
--rw-r--r--   0 nino      (1000) nino      (1000)       89 2024-03-22 09:59:48.000000 django-rahavard-0.0.16/pyproject.toml
--rw-r--r--   0 nino      (1000) nino      (1000)      830 2024-03-28 20:06:16.900889 django-rahavard-0.0.16/setup.cfg
--rw-r--r--   0 nino      (1000) nino      (1000)       38 2024-03-22 10:07:12.000000 django-rahavard-0.0.16/setup.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-06 03:04:59.362782 django-rahavard-0.0.17/
+-rw-r--r--   0 nino      (1000) nino      (1000)     1072 2024-03-22 09:57:46.000000 django-rahavard-0.0.17/LICENSE
+-rw-r--r--   0 nino      (1000) nino      (1000)      897 2024-04-06 03:04:59.362782 django-rahavard-0.0.17/PKG-INFO
+-rw-r--r--   0 nino      (1000) nino      (1000)      100 2024-03-22 12:38:40.000000 django-rahavard-0.0.17/README.md
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-06 03:04:59.289446 django-rahavard-0.0.17/django_rahavard/
+-rw-r--r--   0 nino      (1000) nino      (1000)        0 2024-03-22 08:57:54.000000 django-rahavard-0.0.17/django_rahavard/__init__.py
+-rw-r--r--   0 nino      (1000) nino      (1000)      191 2024-03-22 09:50:24.000000 django-rahavard-0.0.17/django_rahavard/apps.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-06 03:04:59.319447 django-rahavard-0.0.17/django_rahavard/management/
+-rw-r--r--   0 nino      (1000) nino      (1000)        0 2024-03-22 08:57:54.000000 django-rahavard-0.0.17/django_rahavard/management/__init__.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-06 03:04:59.356115 django-rahavard-0.0.17/django_rahavard/management/commands/
+-rw-r--r--   0 nino      (1000) nino      (1000)        0 2024-03-22 08:57:54.000000 django-rahavard-0.0.17/django_rahavard/management/commands/__init__.py
+-rw-r--r--   0 nino      (1000) nino      (1000)      650 2024-03-22 08:57:54.000000 django-rahavard-0.0.17/django_rahavard/management/commands/check_deploy.py
+-rw-r--r--   0 nino      (1000) nino      (1000)     1923 2024-03-22 08:57:54.000000 django-rahavard-0.0.17/django_rahavard/management/commands/collectstatic.py
+-rw-r--r--   0 nino      (1000) nino      (1000)     2878 2024-04-04 20:33:03.000000 django-rahavard-0.0.17/django_rahavard/management/commands/dumpdata.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-06 03:04:59.362782 django-rahavard-0.0.17/django_rahavard/migrations/
+-rw-r--r--   0 nino      (1000) nino      (1000)        0 2024-03-22 08:57:54.000000 django-rahavard-0.0.17/django_rahavard/migrations/__init__.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-06 03:04:59.319447 django-rahavard-0.0.17/django_rahavard.egg-info/
+-rw-r--r--   0 nino      (1000) nino      (1000)      897 2024-04-06 03:04:59.000000 django-rahavard-0.0.17/django_rahavard.egg-info/PKG-INFO
+-rw-r--r--   0 nino      (1000) nino      (1000)      576 2024-04-06 03:04:59.000000 django-rahavard-0.0.17/django_rahavard.egg-info/SOURCES.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)        1 2024-04-06 03:04:59.000000 django-rahavard-0.0.17/django_rahavard.egg-info/dependency_links.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)       16 2024-04-06 03:04:59.000000 django-rahavard-0.0.17/django_rahavard.egg-info/requires.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)       16 2024-04-06 03:04:59.000000 django-rahavard-0.0.17/django_rahavard.egg-info/top_level.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)       89 2024-03-22 09:59:48.000000 django-rahavard-0.0.17/pyproject.toml
+-rw-r--r--   0 nino      (1000) nino      (1000)      830 2024-04-06 03:04:59.362782 django-rahavard-0.0.17/setup.cfg
+-rw-r--r--   0 nino      (1000) nino      (1000)       38 2024-03-22 10:07:12.000000 django-rahavard-0.0.17/setup.py
```

### Comparing `django-rahavard-0.0.16/LICENSE` & `django-rahavard-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rahavard-0.0.16/PKG-INFO` & `django-rahavard-0.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rahavard
-Version: 0.0.16
+Version: 0.0.17
 Summary: A Django App Containing Overridden Django Commands
 Author: Davoud Arsalani
 Author-email: d_arsalani@yahoo.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-rahavard-0.0.16/django_rahavard/management/commands/check_deploy.py` & `django-rahavard-0.0.17/django_rahavard/management/commands/check_deploy.py`

 * *Files identical despite different names*

### Comparing `django-rahavard-0.0.16/django_rahavard/management/commands/collectstatic.py` & `django-rahavard-0.0.17/django_rahavard/management/commands/collectstatic.py`

 * *Files identical despite different names*

### Comparing `django-rahavard-0.0.16/django_rahavard/management/commands/dumpdata.py` & `django-rahavard-0.0.17/django_rahavard/management/commands/dumpdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,16 @@
 
         ## rotate --------------
 
         print('getting list of already present fixtures')
         fixtures = get_list_of_files(directory=settings.FIXTURES_DIR, extension=extension)
         print(f'  count: {len(fixtures)}')
 
-        LAST_FIXTURES_TO_SKIP = 240  ## last n fixtures to skip removing
+        ## keep backups for 90 days
+        LAST_FIXTURES_TO_SKIP = 24 * 90  ## last n fixtures to skip removing
         to_be_removed = fixtures[:-LAST_FIXTURES_TO_SKIP]
 
         if to_be_removed:
             to_be_removed__len = len(to_be_removed)
             print(f'{to_be_removed__len} to be removed:')
             for idx, tbr in enumerate(to_be_removed, start=1):
                 print(f' {idx}/{to_be_removed__len}: removing {tbr}')
```

### Comparing `django-rahavard-0.0.16/django_rahavard.egg-info/PKG-INFO` & `django-rahavard-0.0.17/django_rahavard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rahavard
-Version: 0.0.16
+Version: 0.0.17
 Summary: A Django App Containing Overridden Django Commands
 Author: Davoud Arsalani
 Author-email: d_arsalani@yahoo.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-rahavard-0.0.16/django_rahavard.egg-info/SOURCES.txt` & `django-rahavard-0.0.17/django_rahavard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-rahavard-0.0.16/setup.cfg` & `django-rahavard-0.0.17/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-rahavard
-version = 0.0.16
+version = 0.0.17
 description = A Django App Containing Overridden Django Commands
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Davoud Arsalani
 author_email = d_arsalani@yahoo.com
 license = MIT License
 classifiers =
```

