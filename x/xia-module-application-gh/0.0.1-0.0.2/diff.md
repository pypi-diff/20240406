# Comparing `tmp/xia-module-application-gh-0.0.1.tar.gz` & `tmp/xia-module-application-gh-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-application-gh-0.0.1.tar", last modified: Sun Feb 25 19:18:09 2024, max compression
+gzip compressed data, was "xia-module-application-gh-0.0.2.tar", last modified: Sat Apr  6 15:32:27 2024, max compression
```

## Comparing `xia-module-application-gh-0.0.1.tar` & `xia-module-application-gh-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:18:09.186293 xia-module-application-gh-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-25 19:17:59.000000 xia-module-application-gh-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-25 19:18:08.000000 xia-module-application-gh-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-25 19:18:09.186293 xia-module-application-gh-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 19:17:59.000000 xia-module-application-gh-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 19:18:09.186293 xia-module-application-gh-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-02-25 19:17:59.000000 xia-module-application-gh-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:18:09.186293 xia-module-application-gh-0.0.1/xia_module_application_gh/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-25 19:17:59.000000 xia-module-application-gh-0.0.1/xia_module_application_gh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 19:17:59.000000 xia-module-application-gh-0.0.1/xia_module_application_gh/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:18:09.186293 xia-module-application-gh-0.0.1/xia_module_application_gh/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:18:09.186293 xia-module-application-gh-0.0.1/xia_module_application_gh/templates/gh-module-application/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:18:09.186293 xia-module-application-gh-0.0.1/xia_module_application_gh/templates/gh-module-application/base/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-25 19:17:59.000000 xia-module-application-gh-0.0.1/xia_module_application_gh/templates/gh-module-application/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:18:09.186293 xia-module-application-gh-0.0.1/xia_module_application_gh/templates/gh-module-application/module/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-02-25 19:17:59.000000 xia-module-application-gh-0.0.1/xia_module_application_gh/templates/gh-module-application/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-25 19:17:59.000000 xia-module-application-gh-0.0.1/xia_module_application_gh/templates/gh-module-application/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:18:09.186293 xia-module-application-gh-0.0.1/xia_module_application_gh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-25 19:18:09.000000 xia-module-application-gh-0.0.1/xia_module_application_gh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-25 19:18:09.000000 xia-module-application-gh-0.0.1/xia_module_application_gh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 19:18:09.000000 xia-module-application-gh-0.0.1/xia_module_application_gh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-25 19:18:09.000000 xia-module-application-gh-0.0.1/xia_module_application_gh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 19:18:09.000000 xia-module-application-gh-0.0.1/xia_module_application_gh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:32:27.771516 xia-module-application-gh-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 15:32:16.000000 xia-module-application-gh-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 15:32:27.000000 xia-module-application-gh-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-06 15:32:27.771516 xia-module-application-gh-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 15:32:16.000000 xia-module-application-gh-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:32:27.771516 xia-module-application-gh-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 15:32:16.000000 xia-module-application-gh-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:32:27.767516 xia-module-application-gh-0.0.2/xia_module_application_gh/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-06 15:32:16.000000 xia-module-application-gh-0.0.2/xia_module_application_gh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-06 15:32:16.000000 xia-module-application-gh-0.0.2/xia_module_application_gh/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:32:27.767516 xia-module-application-gh-0.0.2/xia_module_application_gh/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:32:27.767516 xia-module-application-gh-0.0.2/xia_module_application_gh/templates/gh-module-application/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:32:27.767516 xia-module-application-gh-0.0.2/xia_module_application_gh/templates/gh-module-application/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-06 15:32:16.000000 xia-module-application-gh-0.0.2/xia_module_application_gh/templates/gh-module-application/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:32:27.771516 xia-module-application-gh-0.0.2/xia_module_application_gh/templates/gh-module-application/module/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-06 15:32:16.000000 xia-module-application-gh-0.0.2/xia_module_application_gh/templates/gh-module-application/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 15:32:16.000000 xia-module-application-gh-0.0.2/xia_module_application_gh/templates/gh-module-application/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:32:27.767516 xia-module-application-gh-0.0.2/xia_module_application_gh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-06 15:32:27.000000 xia-module-application-gh-0.0.2/xia_module_application_gh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-06 15:32:27.000000 xia-module-application-gh-0.0.2/xia_module_application_gh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:32:27.000000 xia-module-application-gh-0.0.2/xia_module_application_gh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 15:32:27.000000 xia-module-application-gh-0.0.2/xia_module_application_gh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 15:32:27.000000 xia-module-application-gh-0.0.2/xia_module_application_gh.egg-info/top_level.txt
```

### Comparing `xia-module-application-gh-0.0.1/LICENSE` & `xia-module-application-gh-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-application-gh-0.0.1/setup.py` & `xia-module-application-gh-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-application-gh-0.0.1/xia_module_application_gh/templates/gh-module-application/module/main.tf` & `xia-module-application-gh-0.0.2/xia_module_application_gh/templates/gh-module-application/module/main.tf`

 * *Files identical despite different names*

### Comparing `xia-module-application-gh-0.0.1/xia_module_application_gh.egg-info/SOURCES.txt` & `xia-module-application-gh-0.0.2/xia_module_application_gh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

