# Comparing `tmp/dekpkglock-0.1.0.tar.gz` & `tmp/dekpkglock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekpkglock-0.1.0.tar", last modified: Fri Apr  5 18:41:24 2024, max compression
+gzip compressed data, was "dekpkglock-0.1.1.tar", last modified: Sat Apr  6 12:12:07 2024, max compression
```

## Comparing `dekpkglock-0.1.0.tar` & `dekpkglock-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      123 2024-04-05 18:41:23.501261 dekpkglock-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-05 18:41:23.501261 dekpkglock-0.1.0/dekpkglock/__init__.py
--rw-r--r--   0        0        0       42 2024-04-05 18:41:23.501261 dekpkglock-0.1.0/dekpkglock/click/__entry__.py
--rw-r--r--   0        0        0      323 2024-04-05 18:41:23.501261 dekpkglock-0.1.0/dekpkglock/click/__init__.py
--rw-r--r--   0        0        0      216 2024-04-05 18:41:23.501261 dekpkglock-0.1.0/dekpkglock/core/__init__.py
--rw-r--r--   0        0        0     1995 2024-04-05 18:41:23.501261 dekpkglock-0.1.0/dekpkglock/core/base/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-05 18:41:23.501261 dekpkglock-0.1.0/dekpkglock/core/pdm.py
--rw-r--r--   0        0        0   140317 2024-04-05 18:41:23.505261 dekpkglock-0.1.0/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock
--rw-r--r--   0        0        0    31259 2024-04-05 18:41:23.505261 dekpkglock-0.1.0/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock
--rw-r--r--   0        0        0   123953 2024-04-05 18:41:23.505261 dekpkglock-0.1.0/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock
--rw-r--r--   0        0        0      476 2024-04-05 18:41:24.853257 dekpkglock-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 dekpkglock-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-04-06 12:12:06.501307 dekpkglock-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 12:12:06.501307 dekpkglock-0.1.1/dekpkglock/__init__.py
+-rw-r--r--   0        0        0       42 2024-04-06 12:12:06.501307 dekpkglock-0.1.1/dekpkglock/click/__entry__.py
+-rw-r--r--   0        0        0      359 2024-04-06 12:12:06.501307 dekpkglock-0.1.1/dekpkglock/click/__init__.py
+-rw-r--r--   0        0        0      223 2024-04-06 12:12:06.505307 dekpkglock-0.1.1/dekpkglock/core/__init__.py
+-rw-r--r--   0        0        0     2047 2024-04-06 12:12:06.505307 dekpkglock-0.1.1/dekpkglock/core/base/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-06 12:12:06.505307 dekpkglock-0.1.1/dekpkglock/core/pdm.py
+-rw-r--r--   0        0        0   140317 2024-04-06 12:12:06.505307 dekpkglock-0.1.1/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock
+-rw-r--r--   0        0        0   140317 2024-04-06 12:12:06.505307 dekpkglock-0.1.1/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock
+-rw-r--r--   0        0        0    31259 2024-04-06 12:12:06.505307 dekpkglock-0.1.1/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock
+-rw-r--r--   0        0        0   123953 2024-04-06 12:12:06.509307 dekpkglock-0.1.1/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock
+-rw-r--r--   0        0        0      476 2024-04-06 12:12:07.817301 dekpkglock-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 dekpkglock-0.1.1/PKG-INFO
```

### Comparing `dekpkglock-0.1.0/dekpkglock/core/base/__init__.py` & `dekpkglock-0.1.1/dekpkglock/core/base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,18 @@
     name = None
     module_name = __name__.partition(".")[0]
     package_file = None
     lock_file = None
     path_resources = [Path(__file__).resolve().parent.parent.parent / 'resources']
 
     def lock(self, path):
-        for k, v in self.resolve_package_lock(path).items():
+        result = self.resolve_package_lock(path)
+        for k, v in result.items():
             self.lock_package(k, v)
+        return bool(result)
 
     def patch(self, path, index=0):
         unique = set()
         for fp, lock_file in self.find_package_lock(path):
             if lock_file not in unique and lock_file.startswith(str(self.path_resources[index])):
                 self.patch_lock(fp, lock_file)
                 unique.add(lock_file)
```

### Comparing `dekpkglock-0.1.0/dekpkglock/core/pdm.py` & `dekpkglock-0.1.1/dekpkglock/core/pdm.py`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.0/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock` & `dekpkglock-0.1.1/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.0/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock` & `dekpkglock-0.1.1/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.0/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock` & `dekpkglock-0.1.1/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock`

 * *Files identical despite different names*

