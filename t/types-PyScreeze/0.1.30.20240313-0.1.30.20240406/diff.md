# Comparing `tmp/types-PyScreeze-0.1.30.20240313.tar.gz` & `tmp/types-PyScreeze-0.1.30.20240406.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-PyScreeze-0.1.30.20240313.tar", last modified: Wed Mar 13 02:15:19 2024, max compression
+gzip compressed data, was "types-PyScreeze-0.1.30.20240406.tar", last modified: Sat Apr  6 02:13:32 2024, max compression
```

## Comparing `types-PyScreeze-0.1.30.20240313.tar` & `types-PyScreeze-0.1.30.20240406.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 02:15:19.517392 types-PyScreeze-0.1.30.20240313/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-13 02:15:19.000000 types-PyScreeze-0.1.30.20240313/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-13 02:15:19.000000 types-PyScreeze-0.1.30.20240313/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-13 02:15:19.517392 types-PyScreeze-0.1.30.20240313/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 02:15:19.517392 types-PyScreeze-0.1.30.20240313/pyscreeze-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-13 02:15:19.000000 types-PyScreeze-0.1.30.20240313/pyscreeze-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-03-13 02:14:59.000000 types-PyScreeze-0.1.30.20240313/pyscreeze-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 02:15:19.517392 types-PyScreeze-0.1.30.20240313/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-03-13 02:15:19.000000 types-PyScreeze-0.1.30.20240313/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 02:15:19.517392 types-PyScreeze-0.1.30.20240313/types_PyScreeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-13 02:15:19.000000 types-PyScreeze-0.1.30.20240313/types_PyScreeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-13 02:15:19.000000 types-PyScreeze-0.1.30.20240313/types_PyScreeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 02:15:19.000000 types-PyScreeze-0.1.30.20240313/types_PyScreeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-13 02:15:19.000000 types-PyScreeze-0.1.30.20240313/types_PyScreeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-13 02:15:19.000000 types-PyScreeze-0.1.30.20240313/types_PyScreeze.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:32.782631 types-PyScreeze-0.1.30.20240406/
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-06 02:13:32.000000 types-PyScreeze-0.1.30.20240406/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-06 02:13:32.000000 types-PyScreeze-0.1.30.20240406/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-06 02:13:32.782631 types-PyScreeze-0.1.30.20240406/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:32.782631 types-PyScreeze-0.1.30.20240406/pyscreeze-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-06 02:13:32.000000 types-PyScreeze-0.1.30.20240406/pyscreeze-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-06 02:12:57.000000 types-PyScreeze-0.1.30.20240406/pyscreeze-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:32.000000 types-PyScreeze-0.1.30.20240406/pyscreeze-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:13:32.782631 types-PyScreeze-0.1.30.20240406/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-06 02:13:32.000000 types-PyScreeze-0.1.30.20240406/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:32.782631 types-PyScreeze-0.1.30.20240406/types_PyScreeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-06 02:13:32.000000 types-PyScreeze-0.1.30.20240406/types_PyScreeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-06 02:13:32.000000 types-PyScreeze-0.1.30.20240406/types_PyScreeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:13:32.000000 types-PyScreeze-0.1.30.20240406/types_PyScreeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 02:13:32.000000 types-PyScreeze-0.1.30.20240406/types_PyScreeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 02:13:32.000000 types-PyScreeze-0.1.30.20240406/types_PyScreeze.egg-info/top_level.txt
```

### Comparing `types-PyScreeze-0.1.30.20240313/CHANGELOG.md` & `types-PyScreeze-0.1.30.20240406/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.1.30.20240406 (2024-04-06)
+
+Depend on Pillow instead of types-Pillow (#11720)
+
 ## 0.1.30.20240313 (2024-03-13)
 
 Make stubtest work on pyscreeze if you're using py312 (#11582)
 
 ## 0.1.30.20240106 (2024-01-06)
 
 Update typing_extensions imports in third-party stubs (#11245)
```

### Comparing `types-PyScreeze-0.1.30.20240313/PKG-INFO` & `types-PyScreeze-0.1.30.20240406/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyScreeze
-Version: 0.1.30.20240313
+Version: 0.1.30.20240406
 Summary: Typing stubs for PyScreeze
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyScreeze.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-PyScreeze` aims to provide accurate annotations
 for `PyScreeze==0.1.30`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyScreeze. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8a9dcb1967b99600ced8eb4fa6c07df686d09697` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `a9d644b3ffd9e9a8bb9a01393674972573cd256b` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
```

### Comparing `types-PyScreeze-0.1.30.20240313/pyscreeze-stubs/__init__.pyi` & `types-PyScreeze-0.1.30.20240406/pyscreeze-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-PyScreeze-0.1.30.20240313/setup.py` & `types-PyScreeze-0.1.30.20240406/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-PyScreeze` aims to provide accurate annotations
 for `PyScreeze==0.1.30`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyScreeze. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8a9dcb1967b99600ced8eb4fa6c07df686d09697` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `a9d644b3ffd9e9a8bb9a01393674972573cd256b` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="0.1.30.20240313",
+      version="0.1.30.20240406",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyScreeze.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
-      install_requires=['types-Pillow'],
+      install_requires=['Pillow>=10.3.0'],
       packages=['pyscreeze-stubs'],
-      package_data={'pyscreeze-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'pyscreeze-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-PyScreeze-0.1.30.20240313/types_PyScreeze.egg-info/PKG-INFO` & `types-PyScreeze-0.1.30.20240406/types_PyScreeze.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyScreeze
-Version: 0.1.30.20240313
+Version: 0.1.30.20240406
 Summary: Typing stubs for PyScreeze
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyScreeze.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-PyScreeze` aims to provide accurate annotations
 for `PyScreeze==0.1.30`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyScreeze. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8a9dcb1967b99600ced8eb4fa6c07df686d09697` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `a9d644b3ffd9e9a8bb9a01393674972573cd256b` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
```

