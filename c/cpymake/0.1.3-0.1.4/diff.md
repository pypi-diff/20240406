# Comparing `tmp/cpymake-0.1.3.tar.gz` & `tmp/cpymake-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpymake-0.1.3.tar", last modified: Sat Apr  6 02:21:39 2024, max compression
+gzip compressed data, was "cpymake-0.1.4.tar", last modified: Sat Apr  6 02:24:07 2024, max compression
```

## Comparing `cpymake-0.1.3.tar` & `cpymake-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 02:21:39.057768 cpymake-0.1.3/
--rw-rw-rw-   0        0        0    35823 2022-02-23 09:52:53.000000 cpymake-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    45885 2024-04-06 02:21:39.057768 cpymake-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4060 2024-04-02 00:10:44.000000 cpymake-0.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-06 02:21:39.026940 cpymake-0.1.3/cpymake/
--rw-rw-rw-   0        0        0      111 2024-04-05 23:31:11.000000 cpymake-0.1.3/cpymake/__init__.py
--rw-rw-rw-   0        0        0    12986 2024-04-06 02:20:38.000000 cpymake-0.1.3/cpymake/cpymake_build_ext.py
--rw-rw-rw-   0        0        0     2610 2024-04-05 23:49:42.000000 cpymake-0.1.3/cpymake/cpymake_extension.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:21:39.057768 cpymake-0.1.3/cpymake.egg-info/
--rw-rw-rw-   0        0        0    45885 2024-04-06 02:21:39.000000 cpymake-0.1.3/cpymake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-04-06 02:21:39.000000 cpymake-0.1.3/cpymake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 02:21:39.000000 cpymake-0.1.3/cpymake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-06 02:21:39.000000 cpymake-0.1.3/cpymake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-06 02:21:39.000000 cpymake-0.1.3/cpymake.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 02:21:39.057768 cpymake-0.1.3/docs/
--rw-rw-rw-   0        0        0     2065 2023-10-07 14:47:33.000000 cpymake-0.1.3/docs/conf.py
--rw-rw-rw-   0        0        0     1095 2024-04-06 02:21:06.000000 cpymake-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 02:21:39.057768 cpymake-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 02:24:07.125668 cpymake-0.1.4/
+-rw-rw-rw-   0        0        0    35823 2022-02-23 09:52:53.000000 cpymake-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    45885 2024-04-06 02:24:07.125668 cpymake-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2024-04-02 00:10:44.000000 cpymake-0.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-06 02:24:07.094358 cpymake-0.1.4/cpymake/
+-rw-rw-rw-   0        0        0      111 2024-04-05 23:31:11.000000 cpymake-0.1.4/cpymake/__init__.py
+-rw-rw-rw-   0        0        0    13056 2024-04-06 02:23:31.000000 cpymake-0.1.4/cpymake/cpymake_build_ext.py
+-rw-rw-rw-   0        0        0     2610 2024-04-05 23:49:42.000000 cpymake-0.1.4/cpymake/cpymake_extension.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:24:07.125668 cpymake-0.1.4/cpymake.egg-info/
+-rw-rw-rw-   0        0        0    45885 2024-04-06 02:24:07.000000 cpymake-0.1.4/cpymake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-04-06 02:24:07.000000 cpymake-0.1.4/cpymake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 02:24:07.000000 cpymake-0.1.4/cpymake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-06 02:24:07.000000 cpymake-0.1.4/cpymake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-06 02:24:07.000000 cpymake-0.1.4/cpymake.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 02:24:07.125668 cpymake-0.1.4/docs/
+-rw-rw-rw-   0        0        0     2065 2023-10-07 14:47:33.000000 cpymake-0.1.4/docs/conf.py
+-rw-rw-rw-   0        0        0     1095 2024-04-06 02:23:57.000000 cpymake-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 02:24:07.125668 cpymake-0.1.4/setup.cfg
```

### Comparing `cpymake-0.1.3/LICENSE` & `cpymake-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.3/PKG-INFO` & `cpymake-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymake
-Version: 0.1.3
+Version: 0.1.4
 Summary: Allows building of CMake defined Python Extension modules
 Author-email: James Calo <jamesafcalo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cpymake-0.1.3/README.rst` & `cpymake-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.3/cpymake/cpymake_build_ext.py` & `cpymake-0.1.4/cpymake/cpymake_build_ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
             # Config -> outputs in our temp dir
             print(
                 "----- Configure:\n",
                 subprocess.run(
                     ["cmake", extension.cmake_lists_root_dir, *cmake_args],
                     # cwd=self.build_temp,
-                    check=True,
+                    # check=True,
                     capture_output=True,
                 ),
             )
 
             print("~~~~~~~ CWD=", os.getcwd())
 
             # Build -> builds the config (AKA generated solution/makefiles) in
@@ -254,15 +254,17 @@
                 build_cmd.append(f"-j {self.parallel}")
             else:
                 build_cmd.append("-j")
 
             print("##### pre-run")
             print(
                 "----- Configure:\n",
-                subprocess.run(build_cmd, check=True)  # cwd=self.build_temp,
+                subprocess.run(build_cmd, 
+                               # check=True
+                               )  # cwd=self.build_temp,
             )
             print("##### post-run")
 
     # TODO: These three functions need a rewrite! I think we can use special cmake
     # runs, unfortunatly I'm not 100% sure plus it may well
     # be considered "a side affect" although not really? but i guess configure is
     # required
```

### Comparing `cpymake-0.1.3/cpymake/cpymake_extension.py` & `cpymake-0.1.4/cpymake/cpymake_extension.py`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.3/cpymake.egg-info/PKG-INFO` & `cpymake-0.1.4/cpymake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymake
-Version: 0.1.3
+Version: 0.1.4
 Summary: Allows building of CMake defined Python Extension modules
 Author-email: James Calo <jamesafcalo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cpymake-0.1.3/docs/conf.py` & `cpymake-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.3/pyproject.toml` & `cpymake-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpymake"
-version = "0.1.3"
+version = "0.1.4"
 readme = "README.rst"
 description = "Allows building of CMake defined Python Extension modules"
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
 authors = [
     {name = "James Calo", email = "jamesafcalo@gmail.com"},
 ]
```

