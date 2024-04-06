# Comparing `tmp/cdk-events-notify-2.2.90.tar.gz` & `tmp/cdk-events-notify-2.2.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-events-notify-2.2.90.tar", last modified: Fri Apr  5 00:11:57 2024, max compression
+gzip compressed data, was "cdk-events-notify-2.2.91.tar", last modified: Sat Apr  6 00:11:38 2024, max compression
```

## Comparing `cdk-events-notify-2.2.90.tar` & `cdk-events-notify-2.2.91.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:11:57.933320 cdk-events-notify-2.2.90/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-05 00:11:47.000000 cdk-events-notify-2.2.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 00:11:47.000000 cdk-events-notify-2.2.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-05 00:11:57.933320 cdk-events-notify-2.2.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-05 00:11:47.000000 cdk-events-notify-2.2.90/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 00:11:47.000000 cdk-events-notify-2.2.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:11:57.933320 cdk-events-notify-2.2.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-05 00:11:47.000000 cdk-events-notify-2.2.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:11:57.929320 cdk-events-notify-2.2.90/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:11:57.929320 cdk-events-notify-2.2.90/src/cdk_events_notify/
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-05 00:11:47.000000 cdk-events-notify-2.2.90/src/cdk_events_notify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:11:57.933320 cdk-events-notify-2.2.90/src/cdk_events_notify/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-05 00:11:47.000000 cdk-events-notify-2.2.90/src/cdk_events_notify/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-04-05 00:11:47.000000 cdk-events-notify-2.2.90/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.90.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:11:47.000000 cdk-events-notify-2.2.90/src/cdk_events_notify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:11:57.933320 cdk-events-notify-2.2.90/src/cdk_events_notify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-05 00:11:57.000000 cdk-events-notify-2.2.90/src/cdk_events_notify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-05 00:11:57.000000 cdk-events-notify-2.2.90/src/cdk_events_notify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:11:57.000000 cdk-events-notify-2.2.90/src/cdk_events_notify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 00:11:57.000000 cdk-events-notify-2.2.90/src/cdk_events_notify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 00:11:57.000000 cdk-events-notify-2.2.90/src/cdk_events_notify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/src/cdk_events_notify/
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/src/cdk_events_notify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/src/cdk_events_notify/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/src/cdk_events_notify/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24937 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.91.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/src/cdk_events_notify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-06 00:11:38.000000 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-06 00:11:38.000000 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:11:38.000000 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-06 00:11:38.000000 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 00:11:38.000000 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/top_level.txt
```

### Comparing `cdk-events-notify-2.2.90/LICENSE` & `cdk-events-notify-2.2.91/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.90/PKG-INFO` & `cdk-events-notify-2.2.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-events-notify
-Version: 2.2.90
+Version: 2.2.91
 Summary: The Events Notify AWS Construct lib for AWS CDK
 Home-page: https://github.com/neilkuan/cdk-events-notify.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-events-notify.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-events-notify-2.2.90/README.md` & `cdk-events-notify-2.2.91/README.md`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.90/setup.py` & `cdk-events-notify-2.2.91/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-events-notify",
-    "version": "2.2.90",
+    "version": "2.2.91",
     "description": "The Events Notify AWS Construct lib for AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-events-notify.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_events_notify",
         "cdk_events_notify._jsii"
     ],
     "package_data": {
         "cdk_events_notify._jsii": [
-            "cdk-events-notify@2.2.90.jsii.tgz"
+            "cdk-events-notify@2.2.91.jsii.tgz"
         ],
         "cdk_events_notify": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-events-notify-2.2.90/src/cdk_events_notify/__init__.py` & `cdk-events-notify-2.2.91/src/cdk_events_notify/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.90/src/cdk_events_notify.egg-info/PKG-INFO` & `cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-events-notify
-Version: 2.2.90
+Version: 2.2.91
 Summary: The Events Notify AWS Construct lib for AWS CDK
 Home-page: https://github.com/neilkuan/cdk-events-notify.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-events-notify.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

