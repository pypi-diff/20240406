# Comparing `tmp/lbt-grasshopper-1.8.4.tar.gz` & `tmp/lbt-grasshopper-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbt-grasshopper-1.8.4.tar", last modified: Thu Mar 28 20:51:11 2024, max compression
+gzip compressed data, was "dist/lbt-grasshopper-1.8.5.tar", last modified: Sat Apr  6 04:56:14 2024, max compression
```

## Comparing `lbt-grasshopper-1.8.4.tar` & `lbt-grasshopper-1.8.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:51:11.000000 lbt-grasshopper-1.8.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:51:11.000000 lbt-grasshopper-1.8.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:51:11.000000 lbt-grasshopper-1.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/CI_STATUS.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-03-28 20:51:11.000000 lbt-grasshopper-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/ci-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)   730519 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/gradients.png
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/installer.gh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:51:11.000000 lbt-grasshopper-1.8.4/lbt_grasshopper/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/lbt_grasshopper/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:51:11.000000 lbt-grasshopper-1.8.4/lbt_grasshopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-03-28 20:51:10.000000 lbt-grasshopper-1.8.4/lbt_grasshopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-28 20:51:11.000000 lbt-grasshopper-1.8.4/lbt_grasshopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 20:51:10.000000 lbt-grasshopper-1.8.4/lbt_grasshopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-28 20:51:10.000000 lbt-grasshopper-1.8.4/lbt_grasshopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 20:51:10.000000 lbt-grasshopper-1.8.4/lbt_grasshopper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/pass_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/ruby-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-28 20:51:11.000000 lbt-grasshopper-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-03-28 20:50:07.000000 lbt-grasshopper-1.8.4/uninstaller.gh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/CI_STATUS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/ci-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   730519 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/gradients.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/installer.gh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/lbt_grasshopper/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/lbt_grasshopper/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/lbt_grasshopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/lbt_grasshopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/lbt_grasshopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/lbt_grasshopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/lbt_grasshopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/lbt_grasshopper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/pass_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/ruby-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 04:56:14.000000 lbt-grasshopper-1.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-06 04:55:19.000000 lbt-grasshopper-1.8.5/uninstaller.gh
```

### Comparing `lbt-grasshopper-1.8.4/.github/workflows/ci.yaml` & `lbt-grasshopper-1.8.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.4/.github/workflows/dependency-release.yaml` & `lbt-grasshopper-1.8.5/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.4/CI_STATUS.md` & `lbt-grasshopper-1.8.5/CI_STATUS.md`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.4/LICENSE` & `lbt-grasshopper-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.4/PKG-INFO` & `lbt-grasshopper-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-grasshopper
-Version: 1.8.4
+Version: 1.8.5
 Summary: Collection of all Ladybug Tools plugins for Grasshopper
 Home-page: https://github.com/ladybug-tools/lbt-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: IronPython
```

### Comparing `lbt-grasshopper-1.8.4/README.md` & `lbt-grasshopper-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.4/gradients.png` & `lbt-grasshopper-1.8.5/gradients.png`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.4/installer.gh` & `lbt-grasshopper-1.8.5/installer.gh`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.4/lbt_grasshopper.egg-info/PKG-INFO` & `lbt-grasshopper-1.8.5/lbt_grasshopper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-grasshopper
-Version: 1.8.4
+Version: 1.8.5
 Summary: Collection of all Ladybug Tools plugins for Grasshopper
 Home-page: https://github.com/ladybug-tools/lbt-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: IronPython
```

### Comparing `lbt-grasshopper-1.8.4/setup.py` & `lbt-grasshopper-1.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.4/uninstaller.gh` & `lbt-grasshopper-1.8.5/uninstaller.gh`

 * *Files identical despite different names*

