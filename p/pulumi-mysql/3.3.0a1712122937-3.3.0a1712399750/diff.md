# Comparing `tmp/pulumi_mysql-3.3.0a1712122937.tar.gz` & `tmp/pulumi_mysql-3.3.0a1712399750.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_mysql-3.3.0a1712122937.tar", last modified: Wed Apr  3 05:44:39 2024, max compression
+gzip compressed data, was "pulumi_mysql-3.3.0a1712399750.tar", last modified: Sat Apr  6 10:46:09 2024, max compression
```

## Comparing `pulumi_mysql-3.3.0a1712122937.tar` & `pulumi_mysql-3.3.0a1712399750.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:44:39.579756 pulumi_mysql-3.3.0a1712122937/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-03 05:44:39.579756 pulumi_mysql-3.3.0a1712122937/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:44:39.575756 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:44:39.579756 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    27364 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/grant.py
--rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    23843 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql/user_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:44:39.579756 pulumi_mysql-3.3.0a1712122937/pulumi_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-03 05:44:39.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-03 05:44:39.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:44:39.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 05:44:39.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 05:44:39.000000 pulumi_mysql-3.3.0a1712122937/pulumi_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 05:44:33.000000 pulumi_mysql-3.3.0a1712122937/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:44:39.579756 pulumi_mysql-3.3.0a1712122937/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:46:09.601547 pulumi_mysql-3.3.0a1712399750/
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-06 10:46:09.601547 pulumi_mysql-3.3.0a1712399750/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:46:09.597547 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:46:09.601547 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27364 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23843 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql/user_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:46:09.601547 pulumi_mysql-3.3.0a1712399750/pulumi_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-06 10:46:09.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-06 10:46:09.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:46:09.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 10:46:09.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 10:46:09.000000 pulumi_mysql-3.3.0a1712399750/pulumi_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-06 10:46:02.000000 pulumi_mysql-3.3.0a1712399750/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 10:46:09.601547 pulumi_mysql-3.3.0a1712399750/setup.cfg
```

### Comparing `pulumi_mysql-3.3.0a1712122937/PKG-INFO` & `pulumi_mysql-3.3.0a1712399750/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mysql
-Version: 3.3.0a1712122937
+Version: 3.3.0a1712399750
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi,mysql
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.3.0a1712122937/README.md` & `pulumi_mysql-3.3.0a1712399750/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql/__init__.py` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql/_utilities.py` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql/config/__init__.pyi` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql/config/vars.py` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql/database.py` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql/grant.py` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql/grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql/provider.py` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql/role.py` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql/user.py` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql/user_password.py` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql/user_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql.egg-info/PKG-INFO` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mysql
-Version: 3.3.0a1712122937
+Version: 3.3.0a1712399750
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi,mysql
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.3.0a1712122937/pulumi_mysql.egg-info/SOURCES.txt` & `pulumi_mysql-3.3.0a1712399750/pulumi_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1712122937/pyproject.toml` & `pulumi_mysql-3.3.0a1712399750/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_mysql"
   description = "A Pulumi package for creating and managing mysql cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0a1,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "mysql"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.3.0a1712122937"
+  version = "3.3.0a1712399750"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-mysql"
 
 [build-system]
```

