# Comparing `tmp/django-denied-1.2.tar.gz` & `tmp/django-denied-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-denied-1.2.tar", last modified: Mon Sep  5 01:05:58 2022, max compression
+gzip compressed data, was "django-denied-1.3.tar", last modified: Sat Apr  6 17:42:53 2024, max compression
```

## Comparing `django-denied-1.2.tar` & `django-denied-1.3.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2022-09-05 01:05:58.000788 django-denied-1.2/
--rw-r--r--   0 matt       (501) staff       (20)     1068 2022-07-28 01:14:05.000000 django-denied-1.2/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)       85 2022-07-28 05:27:41.000000 django-denied-1.2/MANIFEST.in
--rw-r--r--   0 matt       (501) staff       (20)     8852 2022-09-05 01:05:58.000946 django-denied-1.2/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     7867 2022-09-04 19:50:20.000000 django-denied-1.2/README.md
--rw-r--r--   0 matt       (501) staff       (20)      735 2022-07-28 05:09:12.000000 django-denied-1.2/pyproject.toml
--rw-r--r--   0 matt       (501) staff       (20)     1261 2022-09-05 01:05:58.001735 django-denied-1.2/setup.cfg
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2022-09-05 01:05:57.995801 django-denied-1.2/src/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2022-09-05 01:05:57.999034 django-denied-1.2/src/denied/
--rw-r--r--   0 matt       (501) staff       (20)        0 2022-07-28 01:52:40.000000 django-denied-1.2/src/denied/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)      358 2022-07-28 05:19:20.000000 django-denied-1.2/src/denied/authorizers.py
--rw-r--r--   0 matt       (501) staff       (20)     2360 2022-07-28 05:11:03.000000 django-denied-1.2/src/denied/decorators.py
--rw-r--r--   0 matt       (501) staff       (20)     1828 2022-09-05 01:05:13.000000 django-denied-1.2/src/denied/middleware.py
--rw-r--r--   0 matt       (501) staff       (20)        0 2022-07-28 05:11:49.000000 django-denied-1.2/src/denied/py.typed
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2022-09-05 01:05:58.000474 django-denied-1.2/src/django_denied.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     8852 2022-09-05 01:05:57.000000 django-denied-1.2/src/django_denied.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      377 2022-09-05 01:05:57.000000 django-denied-1.2/src/django_denied.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2022-09-05 01:05:57.000000 django-denied-1.2/src/django_denied.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)       12 2022-09-05 01:05:57.000000 django-denied-1.2/src/django_denied.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)        7 2022-09-05 01:05:57.000000 django-denied-1.2/src/django_denied.egg-info/top_level.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-04-06 17:42:53.036211 django-denied-1.3/
+-rw-r--r--   0 matt       (501) staff       (20)     1068 2022-07-28 01:14:05.000000 django-denied-1.3/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)       85 2022-07-28 05:27:41.000000 django-denied-1.3/MANIFEST.in
+-rw-r--r--   0 matt       (501) staff       (20)     9009 2024-04-06 17:42:53.035807 django-denied-1.3/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     7867 2022-09-04 19:50:20.000000 django-denied-1.3/README.md
+-rw-r--r--   0 matt       (501) staff       (20)      735 2022-07-28 05:09:12.000000 django-denied-1.3/pyproject.toml
+-rw-r--r--   0 matt       (501) staff       (20)     1364 2024-04-06 17:42:53.037363 django-denied-1.3/setup.cfg
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-04-06 17:42:53.022835 django-denied-1.3/src/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-04-06 17:42:53.029788 django-denied-1.3/src/denied/
+-rw-r--r--   0 matt       (501) staff       (20)        0 2022-07-28 01:52:40.000000 django-denied-1.3/src/denied/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)      358 2022-07-28 05:19:20.000000 django-denied-1.3/src/denied/authorizers.py
+-rw-r--r--   0 matt       (501) staff       (20)     2332 2024-04-06 16:01:43.000000 django-denied-1.3/src/denied/decorators.py
+-rw-r--r--   0 matt       (501) staff       (20)     1916 2024-04-06 16:19:01.000000 django-denied-1.3/src/denied/middleware.py
+-rw-r--r--   0 matt       (501) staff       (20)        0 2022-07-28 05:11:49.000000 django-denied-1.3/src/denied/py.typed
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-04-06 17:42:53.034966 django-denied-1.3/src/django_denied.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)     9009 2024-04-06 17:42:53.000000 django-denied-1.3/src/django_denied.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      453 2024-04-06 17:42:53.000000 django-denied-1.3/src/django_denied.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2024-04-06 17:42:53.000000 django-denied-1.3/src/django_denied.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)       12 2024-04-06 17:42:53.000000 django-denied-1.3/src/django_denied.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)        7 2024-04-06 17:42:53.000000 django-denied-1.3/src/django_denied.egg-info/top_level.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-04-06 17:42:53.033973 django-denied-1.3/tests/
+-rw-r--r--   0 matt       (501) staff       (20)      676 2022-07-28 05:19:20.000000 django-denied-1.3/tests/test_authorizers.py
+-rw-r--r--   0 matt       (501) staff       (20)     4394 2022-09-05 01:05:13.000000 django-denied-1.3/tests/test_decorators.py
+-rw-r--r--   0 matt       (501) staff       (20)     5265 2024-04-06 16:28:03.000000 django-denied-1.3/tests/test_middleware.py
```

### Comparing `django-denied-1.2/LICENSE` & `django-denied-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-denied-1.2/PKG-INFO` & `django-denied-1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: django-denied
-Version: 1.2
+Version: 1.3
 Summary: An authorization system based exclusively on allow lists
 Home-page: https://github.com/mblayman/django-denied
 Author: Matt Layman
 Author-email: matthewlayman@gmail.com
 License: MIT
 Keywords: Django
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=3.2
 
 # django-denied
 
 > None shall pass.
 >
 > The Black Knight
```

### Comparing `django-denied-1.2/README.md` & `django-denied-1.3/README.md`

 * *Files identical despite different names*

### Comparing `django-denied-1.2/pyproject.toml` & `django-denied-1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-denied-1.2/setup.cfg` & `django-denied-1.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [metadata]
 name = django-denied
-version = 1.2
+version = 1.3
 description = An authorization system based exclusively on allow lists
 url = https://github.com/mblayman/django-denied
 license = MIT
 author = Matt Layman
 author_email = matthewlayman@gmail.com
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Django
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
+	Framework :: Django :: 5.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 install_requires = 
@@ -49,13 +52,13 @@
 	.tox/*/site-packages
 
 [coverage:report]
 show_missing = True
 
 [flake8]
 max-line-length = 88
-ignore = E203, W503
+ignore = E203, E704, W503
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-denied-1.2/src/denied/decorators.py` & `django-denied-1.3/src/denied/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,39 +4,36 @@
 from functools import wraps
 from typing import Callable, overload
 
 from django.urls.resolvers import URLPattern, URLResolver
 
 
 @overload
-def allow(view_func: Callable) -> Callable:
-    ...  # pragma: no cover
+def allow(view_func: Callable) -> Callable: ...  # pragma: no cover
 
 
 @overload
-def allow(view_func: list) -> list:
-    ...  # pragma: no cover
+def allow(view_func: list) -> list: ...  # pragma: no cover
 
 
 @overload
-def allow(view_func: tuple) -> tuple:
-    ...  # pragma: no cover
+def allow(view_func: tuple) -> tuple: ...  # pragma: no cover
 
 
 def allow(view_func: Callable | list | tuple) -> Callable | list | tuple:
     """Allow a view without any authorization checking."""
 
     if isinstance(view_func, (list, tuple)):
         _allow_many(view_func)
         return view_func
 
     @wraps(view_func)
     def wrapper(*args, **kwargs):  # type: ignore
         # mypy is ignoring the isinstance check for some reason.
-        return view_func(*args, **kwargs)  # type: ignore
+        return view_func(*args, **kwargs)
 
     wrapper.__denied_exempt__ = True  # type: ignore
     return wrapper
 
 
 def _allow_many(view_func: list | tuple) -> None:
     """Allow many views.
```

### Comparing `django-denied-1.2/src/denied/middleware.py` & `django-denied-1.3/src/denied/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,22 +38,25 @@
         if (
             getattr(view_func, "__denied_exempt__", False)
             # Or check on a bound method
             or getattr(getattr(view_func, "__func__", None), "__denied_exempt__", False)
         ):
             return None
 
+        if settings.MEDIA_URL and request.path.startswith(settings.MEDIA_URL):
+            return None
+
         if not request.user.is_authenticated and request.path not in LOGIN_URLS:
             return redirect_to_login(request.get_full_path())
 
         if not hasattr(view_func, "__denied_authorizer__"):
             # Permit the login URLs always.
             if request.path in LOGIN_URLS:
                 return None
 
             raise PermissionDenied()
 
         # __denied_authorizer__ is set by the various decorators.
-        if not view_func.__denied_authorizer__(request, **view_kwargs):  # type: ignore
+        if not view_func.__denied_authorizer__(request, **view_kwargs):
             raise PermissionDenied()
 
         return None
```

### Comparing `django-denied-1.2/src/django_denied.egg-info/PKG-INFO` & `django-denied-1.3/src/django_denied.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: django-denied
-Version: 1.2
+Version: 1.3
 Summary: An authorization system based exclusively on allow lists
 Home-page: https://github.com/mblayman/django-denied
 Author: Matt Layman
 Author-email: matthewlayman@gmail.com
 License: MIT
 Keywords: Django
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=3.2
 
 # django-denied
 
 > None shall pass.
 >
 > The Black Knight
```

