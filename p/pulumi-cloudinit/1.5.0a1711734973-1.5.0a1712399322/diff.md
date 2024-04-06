# Comparing `tmp/pulumi_cloudinit-1.5.0a1711734973.tar.gz` & `tmp/pulumi_cloudinit-1.5.0a1712399322.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_cloudinit-1.5.0a1711734973.tar", last modified: Fri Mar 29 18:07:54 2024, max compression
+gzip compressed data, was "pulumi_cloudinit-1.5.0a1712399322.tar", last modified: Sat Apr  6 10:42:39 2024, max compression
```

## Comparing `pulumi_cloudinit-1.5.0a1711734973.tar` & `pulumi_cloudinit-1.5.0a1712399322.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:07:54.778854 pulumi_cloudinit-1.5.0a1711734973/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-29 18:07:54.778854 pulumi_cloudinit-1.5.0a1711734973/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:07:54.778854 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:07:54.778854 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-29 18:07:54.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-29 18:07:54.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 18:07:54.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 18:07:54.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-29 18:07:54.000000 pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-29 18:07:48.000000 pulumi_cloudinit-1.5.0a1711734973/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 18:07:54.778854 pulumi_cloudinit-1.5.0a1711734973/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:39.336238 pulumi_cloudinit-1.5.0a1712399322/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-06 10:42:39.336238 pulumi_cloudinit-1.5.0a1712399322/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:39.336238 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:39.336238 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-06 10:42:39.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-06 10:42:39.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:42:39.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 10:42:39.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 10:42:39.000000 pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-06 10:42:32.000000 pulumi_cloudinit-1.5.0a1712399322/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 10:42:39.336238 pulumi_cloudinit-1.5.0a1712399322/setup.cfg
```

### Comparing `pulumi_cloudinit-1.5.0a1711734973/PKG-INFO` & `pulumi_cloudinit-1.5.0a1712399322/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.5.0a1711734973
+Version: 1.5.0a1712399322
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi,cloudinit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.5.0a1711734973/README.md` & `pulumi_cloudinit-1.5.0a1712399322/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/__init__.py` & `pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/_inputs.py` & `pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/_utilities.py` & `pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/config.py` & `pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/get_config.py` & `pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/outputs.py` & `pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit/provider.py` & `pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1711734973/pulumi_cloudinit.egg-info/PKG-INFO` & `pulumi_cloudinit-1.5.0a1712399322/pulumi_cloudinit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.5.0a1711734973
+Version: 1.5.0a1712399322
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi,cloudinit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.5.0a1711734973/pyproject.toml` & `pulumi_cloudinit-1.5.0a1712399322/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_cloudinit"
   description = "A Pulumi package for creating and managing cloudinit cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "cloudinit"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.5.0a1711734973"
+  version = "1.5.0a1712399322"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-cloudinit"
 
 [build-system]
```

