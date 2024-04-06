# Comparing `tmp/cpymake-0.1.0.tar.gz` & `tmp/cpymake-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpymake-0.1.0.tar", last modified: Tue Apr  2 00:11:14 2024, max compression
+gzip compressed data, was "cpymake-0.1.1.tar", last modified: Sat Apr  6 02:08:45 2024, max compression
```

## Comparing `cpymake-0.1.0.tar` & `cpymake-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 00:11:14.749400 cpymake-0.1.0/
--rw-rw-rw-   0        0        0    35823 2022-02-23 09:52:53.000000 cpymake-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    45885 2024-04-02 00:11:14.744098 cpymake-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4060 2024-04-02 00:10:44.000000 cpymake-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-02 00:11:14.693550 cpymake-0.1.0/cpymake/
--rw-rw-rw-   0        0        0        0 2023-10-07 00:44:35.000000 cpymake-0.1.0/cpymake/__init__.py
--rw-rw-rw-   0        0        0     7440 2024-03-11 13:04:20.000000 cpymake-0.1.0/cpymake/cemake_build_ext.py
--rw-rw-rw-   0        0        0     2599 2023-10-07 23:22:59.000000 cpymake-0.1.0/cpymake/cemake_extension.py
-drwxrwxrwx   0        0        0        0 2024-04-02 00:11:14.744098 cpymake-0.1.0/cpymake.egg-info/
--rw-rw-rw-   0        0        0    45885 2024-04-02 00:11:14.000000 cpymake-0.1.0/cpymake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-02 00:11:14.000000 cpymake-0.1.0/cpymake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 00:11:14.000000 cpymake-0.1.0/cpymake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-02 00:11:14.000000 cpymake-0.1.0/cpymake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-02 00:11:14.000000 cpymake-0.1.0/cpymake.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 00:11:14.743379 cpymake-0.1.0/docs/
--rw-rw-rw-   0        0        0     2065 2023-10-07 14:47:33.000000 cpymake-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0     1095 2024-04-02 00:10:52.000000 cpymake-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 00:11:14.749400 cpymake-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 02:08:45.249987 cpymake-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2022-02-23 09:52:53.000000 cpymake-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    45885 2024-04-06 02:08:45.249987 cpymake-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2024-04-02 00:10:44.000000 cpymake-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-06 02:08:45.218660 cpymake-0.1.1/cpymake/
+-rw-rw-rw-   0        0        0      111 2024-04-05 23:31:11.000000 cpymake-0.1.1/cpymake/__init__.py
+-rw-rw-rw-   0        0        0    12858 2024-04-06 01:59:57.000000 cpymake-0.1.1/cpymake/cpymake_build_ext.py
+-rw-rw-rw-   0        0        0     2610 2024-04-05 23:49:42.000000 cpymake-0.1.1/cpymake/cpymake_extension.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:08:45.249987 cpymake-0.1.1/cpymake.egg-info/
+-rw-rw-rw-   0        0        0    45885 2024-04-06 02:08:45.000000 cpymake-0.1.1/cpymake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-04-06 02:08:45.000000 cpymake-0.1.1/cpymake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 02:08:45.000000 cpymake-0.1.1/cpymake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-06 02:08:45.000000 cpymake-0.1.1/cpymake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-06 02:08:45.000000 cpymake-0.1.1/cpymake.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 02:08:45.249987 cpymake-0.1.1/docs/
+-rw-rw-rw-   0        0        0     2065 2023-10-07 14:47:33.000000 cpymake-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0     1095 2024-04-06 02:06:38.000000 cpymake-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 02:08:45.249987 cpymake-0.1.1/setup.cfg
```

### Comparing `cpymake-0.1.0/LICENSE` & `cpymake-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.0/PKG-INFO` & `cpymake-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymake
-Version: 0.1.0
+Version: 0.1.1
 Summary: Allows building of CMake defined Python Extension modules
 Author-email: James Calo <jamesafcalo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cpymake-0.1.0/README.rst` & `cpymake-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.0/cpymake/cemake_extension.py` & `cpymake-0.1.1/cpymake/cpymake_extension.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dataclasses import dataclass
 
 from setuptools import errors
 from setuptools.extension import Extension
 
 
 @dataclass
-class CeMakeExtension(Extension):
+class CPyMakeExtension(Extension):
     """This is the main ``Extension`` class for describing cmake python
     extension module builds.
 
     Attributes
     ----------
     package_name : str
       The name of the package, in dotted notation
@@ -53,15 +53,15 @@
         targets: list[str] | None = None,  # Could make args?
         generator: str | None = None,
         *args,
         **kwargs,
     ):
         super().__init__(name=package_name, sources=[], *args, **kwargs)  # type:ignore
         self.package_name = package_name
-        if not os.path.isabs(cmake_lists_root_dir):
-            raise errors.SetupError(
-                "cmake_lists_root_dir must be an absolute path but recieved:"
-                f" {cmake_lists_root_dir}"
-            )
+        # if not os.path.isabs(cmake_lists_root_dir):
+        #     raise errors.SetupError(
+        #         "cmake_lists_root_dir must be an absolute path but recieved:"
+        #         f" {cmake_lists_root_dir}"
+        #     )
         self.cmake_lists_root_dir = cmake_lists_root_dir
         self.targets = targets
         self.generator = generator
```

### Comparing `cpymake-0.1.0/cpymake.egg-info/PKG-INFO` & `cpymake-0.1.1/cpymake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymake
-Version: 0.1.0
+Version: 0.1.1
 Summary: Allows building of CMake defined Python Extension modules
 Author-email: James Calo <jamesafcalo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cpymake-0.1.0/docs/conf.py` & `cpymake-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.0/pyproject.toml` & `cpymake-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpymake"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 description = "Allows building of CMake defined Python Extension modules"
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
 authors = [
     {name = "James Calo", email = "jamesafcalo@gmail.com"},
 ]
@@ -25,14 +25,14 @@
 [project.urls]
 #Homepage = "https://example.com"
 #Documentation = "https://readthedocs.org"
 Repository = "https://github.com/SagaraBattousai/cpymake.git"
 #Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
 
 [project.entry-points."distutils.commands"]
-cpymake = "cpymake.cpymake_build_ext:cpymakeBuildExt"
+cpymake = "cpymake.cpymake_build_ext:CPyMakeBuildExt"
 
 [tool.setuptools.packages.find]
 exclude = ["docs_build"] # temp
 
 [tool.black]
 preview = true
```

