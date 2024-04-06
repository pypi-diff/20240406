# Comparing `tmp/pypotage-0.0.0a0.tar.gz` & `tmp/pypotage-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypotage-0.0.0a0.tar", last modified: Tue Mar 26 19:54:44 2024, max compression
+gzip compressed data, was "pypotage-0.1.0a0.tar", last modified: Sat Apr  6 08:19:36 2024, max compression
```

## Comparing `pypotage-0.0.0a0.tar` & `pypotage-0.1.0a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:54:44.481082 pypotage-0.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-26 19:54:44.481082 pypotage-0.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:54:37.000000 pypotage-0.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-26 19:54:37.000000 pypotage-0.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-26 19:54:44.481082 pypotage-0.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:54:44.477082 pypotage-0.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:54:44.477082 pypotage-0.0.0a0/src/pypotage/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-26 19:54:37.000000 pypotage-0.0.0a0/src/pypotage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-26 19:54:37.000000 pypotage-0.0.0a0/src/pypotage/_bean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-26 19:54:37.000000 pypotage-0.0.0a0/src/pypotage/_jar.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-26 19:54:37.000000 pypotage-0.0.0a0/src/pypotage/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-26 19:54:37.000000 pypotage-0.0.0a0/src/pypotage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:54:44.481082 pypotage-0.0.0a0/src/pypotage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-26 19:54:44.000000 pypotage-0.0.0a0/src/pypotage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-26 19:54:44.000000 pypotage-0.0.0a0/src/pypotage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:54:44.000000 pypotage-0.0.0a0/src/pypotage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-26 19:54:44.000000 pypotage-0.0.0a0/src/pypotage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:19:36.450472 pypotage-0.1.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 08:19:36.450472 pypotage-0.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-06 08:19:36.454472 pypotage-0.1.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:19:36.450472 pypotage-0.1.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:19:36.450472 pypotage-0.1.0a0/src/pypotage/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/src/pypotage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/src/pypotage/_ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/src/pypotage/_pot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/src/pypotage/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/src/pypotage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:19:36.450472 pypotage-0.1.0a0/src/pypotage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 08:19:36.000000 pypotage-0.1.0a0/src/pypotage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-06 08:19:36.000000 pypotage-0.1.0a0/src/pypotage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 08:19:36.000000 pypotage-0.1.0a0/src/pypotage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 08:19:36.000000 pypotage-0.1.0a0/src/pypotage.egg-info/top_level.txt
```

### Comparing `pypotage-0.0.0a0/PKG-INFO` & `pypotage-0.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypotage
-Version: 0.0.0a0
+Version: 0.1.0a0
 Summary: Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 Home-page: https://github.com/pavalso/potage
 Author: Pavalso
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pavalso/potage/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypotage-0.0.0a0/setup.cfg` & `pypotage-0.1.0a0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pypotage
-version = v0.0.0-alpha
+version = v0.1.0-alpha
 author = Pavalso
 author_email = author@example.com
 description = Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pavalso/potage
 project_urls =
```

### Comparing `pypotage-0.0.0a0/src/pypotage/_bean.py` & `pypotage-0.1.0a0/src/pypotage/_ingredient.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,61 @@
-from typing import Generic, TypeVar, Callable, Type
+from typing import Generic, TypeVar, Callable, Any
 
 from dataclasses import dataclass
 from math import inf
 from inspect import isclass
 
 
 _B = TypeVar("_B")
 
+
 @dataclass(kw_only=True, repr=False)
-class _BeanProxy(Generic[_B]):
+class _IngredientProxy(Generic[_B]):
 
     _f: Callable
 
     def is_present(self) -> bool:
         return bool(self._f())
 
-    def get(self) -> _B:
-        _beans = self._f()
+    def take_out(self) -> _B:
+        _ingredients = self._f()
+
+        if _ingredients == []:
+            raise RuntimeError("No ingredients found")
 
-        return _beans[0]() if _beans else None
+        return _ingredients[0]() if _ingredients else None
 
     def __call__(self) -> _B:
-        return self.get()
+        return self.take_out()
+
 
 @dataclass(kw_only=True, repr=False)
-class _Bean:
+class _Ingredient:
 
     _c: Callable
 
     lazy: bool = False
     order: int = inf
     primary: bool = False
 
     @property
     def priority(self) -> int:
         return -inf if self.primary else self.order
 
     @property
-    def type(self) -> Type:
+    def type(self) -> Any:
         _annotation = self._c.__annotations__.get("return")
 
         if self.lazy:
             if isclass(self._c.__wrapped__):
                 return self._c.__wrapped__
 
             if _annotation is None:
-                raise RuntimeError("Lazy beans must explicitly define their return type")
+                raise RuntimeError("Lazy ingredients must explicitly define their return type")
+
+        if _annotation is not None:
             return _annotation
 
         return type(self._c())
 
     def __call__(self):
         return self._c()
```

### Comparing `pypotage-0.0.0a0/src/pypotage.egg-info/PKG-INFO` & `pypotage-0.1.0a0/src/pypotage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypotage
-Version: 0.0.0a0
+Version: 0.1.0a0
 Summary: Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 Home-page: https://github.com/pavalso/potage
 Author: Pavalso
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pavalso/potage/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

