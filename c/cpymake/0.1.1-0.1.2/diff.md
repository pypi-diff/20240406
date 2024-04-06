# Comparing `tmp/cpymake-0.1.1.tar.gz` & `tmp/cpymake-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpymake-0.1.1.tar", last modified: Sat Apr  6 02:08:45 2024, max compression
+gzip compressed data, was "cpymake-0.1.2.tar", last modified: Sat Apr  6 02:13:14 2024, max compression
```

## Comparing `cpymake-0.1.1.tar` & `cpymake-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 02:08:45.249987 cpymake-0.1.1/
--rw-rw-rw-   0        0        0    35823 2022-02-23 09:52:53.000000 cpymake-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    45885 2024-04-06 02:08:45.249987 cpymake-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4060 2024-04-02 00:10:44.000000 cpymake-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-06 02:08:45.218660 cpymake-0.1.1/cpymake/
--rw-rw-rw-   0        0        0      111 2024-04-05 23:31:11.000000 cpymake-0.1.1/cpymake/__init__.py
--rw-rw-rw-   0        0        0    12858 2024-04-06 01:59:57.000000 cpymake-0.1.1/cpymake/cpymake_build_ext.py
--rw-rw-rw-   0        0        0     2610 2024-04-05 23:49:42.000000 cpymake-0.1.1/cpymake/cpymake_extension.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:08:45.249987 cpymake-0.1.1/cpymake.egg-info/
--rw-rw-rw-   0        0        0    45885 2024-04-06 02:08:45.000000 cpymake-0.1.1/cpymake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-04-06 02:08:45.000000 cpymake-0.1.1/cpymake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 02:08:45.000000 cpymake-0.1.1/cpymake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-06 02:08:45.000000 cpymake-0.1.1/cpymake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-06 02:08:45.000000 cpymake-0.1.1/cpymake.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 02:08:45.249987 cpymake-0.1.1/docs/
--rw-rw-rw-   0        0        0     2065 2023-10-07 14:47:33.000000 cpymake-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0     1095 2024-04-06 02:06:38.000000 cpymake-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 02:08:45.249987 cpymake-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 02:13:14.316888 cpymake-0.1.2/
+-rw-rw-rw-   0        0        0    35823 2022-02-23 09:52:53.000000 cpymake-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    45885 2024-04-06 02:13:14.301270 cpymake-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2024-04-02 00:10:44.000000 cpymake-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-06 02:13:14.285630 cpymake-0.1.2/cpymake/
+-rw-rw-rw-   0        0        0      111 2024-04-05 23:31:11.000000 cpymake-0.1.2/cpymake/__init__.py
+-rw-rw-rw-   0        0        0    12835 2024-04-06 02:11:24.000000 cpymake-0.1.2/cpymake/cpymake_build_ext.py
+-rw-rw-rw-   0        0        0     2610 2024-04-05 23:49:42.000000 cpymake-0.1.2/cpymake/cpymake_extension.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:13:14.301270 cpymake-0.1.2/cpymake.egg-info/
+-rw-rw-rw-   0        0        0    45885 2024-04-06 02:13:14.000000 cpymake-0.1.2/cpymake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-04-06 02:13:14.000000 cpymake-0.1.2/cpymake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 02:13:14.000000 cpymake-0.1.2/cpymake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-06 02:13:14.000000 cpymake-0.1.2/cpymake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-06 02:13:14.000000 cpymake-0.1.2/cpymake.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 02:13:14.301270 cpymake-0.1.2/docs/
+-rw-rw-rw-   0        0        0     2065 2023-10-07 14:47:33.000000 cpymake-0.1.2/docs/conf.py
+-rw-rw-rw-   0        0        0     1095 2024-04-06 02:13:06.000000 cpymake-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 02:13:14.316888 cpymake-0.1.2/setup.cfg
```

### Comparing `cpymake-0.1.1/LICENSE` & `cpymake-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.1/PKG-INFO` & `cpymake-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymake
-Version: 0.1.1
+Version: 0.1.2
 Summary: Allows building of CMake defined Python Extension modules
 Author-email: James Calo <jamesafcalo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cpymake-0.1.1/README.rst` & `cpymake-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.1/cpymake/cpymake_build_ext.py` & `cpymake-0.1.2/cpymake/cpymake_build_ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
             print("******", extension)
             # Looks dodgy but it's been years since I made this so...
             # Actually maybe not...
             # self.package = (  # pylint: disable=attribute-defined-outside-init
             #     extension.package_name
             # )
             # extension_dir = self.get_extension_build_directory(extension.name)
-            extension_dir = os.getcwd() + os.sep + self.build_lib
+            extension_dir = self.build_lib
             extension_suffix = (
                 # self.extension_suffix  # sysconfig.get_config_var("EXT_SUFFIX")
                 sysconfig.get_config_var("EXT_SUFFIX")
             )
 
             # Should I also allow this to be overridable in extension?
             config = "Debug" if self.debug else "Release"
```

### Comparing `cpymake-0.1.1/cpymake/cpymake_extension.py` & `cpymake-0.1.2/cpymake/cpymake_extension.py`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.1/cpymake.egg-info/PKG-INFO` & `cpymake-0.1.2/cpymake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymake
-Version: 0.1.1
+Version: 0.1.2
 Summary: Allows building of CMake defined Python Extension modules
 Author-email: James Calo <jamesafcalo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cpymake-0.1.1/docs/conf.py` & `cpymake-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.1/pyproject.toml` & `cpymake-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpymake"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 description = "Allows building of CMake defined Python Extension modules"
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
 authors = [
     {name = "James Calo", email = "jamesafcalo@gmail.com"},
 ]
```

