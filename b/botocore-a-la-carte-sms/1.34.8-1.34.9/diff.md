# Comparing `tmp/botocore-a-la-carte-sms-1.34.8.tar.gz` & `tmp/botocore-a-la-carte-sms-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-sms-1.34.8.tar", last modified: Wed Dec 27 01:07:02 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-sms-1.34.9.tar", last modified: Thu Dec 28 01:07:04 2023, max compression
```

## Comparing `botocore-a-la-carte-sms-1.34.8.tar` & `botocore-a-la-carte-sms-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:02.675360 botocore-a-la-carte-sms-1.34.8/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-27 01:07:02.000000 botocore-a-la-carte-sms-1.34.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-27 01:07:02.675360 botocore-a-la-carte-sms-1.34.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:02.675360 botocore-a-la-carte-sms-1.34.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:02.675360 botocore-a-la-carte-sms-1.34.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:02.675360 botocore-a-la-carte-sms-1.34.8/botocore/data/sms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:02.675360 botocore-a-la-carte-sms-1.34.8/botocore/data/sms/2016-10-24/
--rw-r--r--   0 runner    (1001) docker     (127)    17612 2023-12-27 01:06:29.000000 botocore-a-la-carte-sms-1.34.8/botocore/data/sms/2016-10-24/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-27 01:06:29.000000 botocore-a-la-carte-sms-1.34.8/botocore/data/sms/2016-10-24/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-27 01:06:29.000000 botocore-a-la-carte-sms-1.34.8/botocore/data/sms/2016-10-24/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    89540 2023-12-27 01:06:29.000000 botocore-a-la-carte-sms-1.34.8/botocore/data/sms/2016-10-24/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:02.675360 botocore-a-la-carte-sms-1.34.8/botocore_a_la_carte_sms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-27 01:07:02.000000 botocore-a-la-carte-sms-1.34.8/botocore_a_la_carte_sms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-27 01:07:02.000000 botocore-a-la-carte-sms-1.34.8/botocore_a_la_carte_sms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 01:07:02.000000 botocore-a-la-carte-sms-1.34.8/botocore_a_la_carte_sms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 01:07:02.000000 botocore-a-la-carte-sms-1.34.8/botocore_a_la_carte_sms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 01:07:02.675360 botocore-a-la-carte-sms-1.34.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-27 01:07:02.000000 botocore-a-la-carte-sms-1.34.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.418457 botocore-a-la-carte-sms-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:07:04.000000 botocore-a-la-carte-sms-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:07:04.418457 botocore-a-la-carte-sms-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.418457 botocore-a-la-carte-sms-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.418457 botocore-a-la-carte-sms-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.418457 botocore-a-la-carte-sms-1.34.9/botocore/data/sms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.418457 botocore-a-la-carte-sms-1.34.9/botocore/data/sms/2016-10-24/
+-rw-r--r--   0 runner    (1001) docker     (127)    17612 2023-12-28 01:06:26.000000 botocore-a-la-carte-sms-1.34.9/botocore/data/sms/2016-10-24/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-sms-1.34.9/botocore/data/sms/2016-10-24/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-28 01:06:26.000000 botocore-a-la-carte-sms-1.34.9/botocore/data/sms/2016-10-24/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    89540 2023-12-28 01:06:26.000000 botocore-a-la-carte-sms-1.34.9/botocore/data/sms/2016-10-24/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.418457 botocore-a-la-carte-sms-1.34.9/botocore_a_la_carte_sms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:07:04.000000 botocore-a-la-carte-sms-1.34.9/botocore_a_la_carte_sms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-28 01:07:04.000000 botocore-a-la-carte-sms-1.34.9/botocore_a_la_carte_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:07:04.000000 botocore-a-la-carte-sms-1.34.9/botocore_a_la_carte_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:07:04.000000 botocore-a-la-carte-sms-1.34.9/botocore_a_la_carte_sms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:07:04.418457 botocore-a-la-carte-sms-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-28 01:07:04.000000 botocore-a-la-carte-sms-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-sms-1.34.8/LICENSE.txt` & `botocore-a-la-carte-sms-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sms-1.34.8/PKG-INFO` & `botocore-a-la-carte-sms-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sms
-Version: 1.34.8
+Version: 1.34.9
 Summary: sms data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sms-1.34.8/botocore/data/sms/2016-10-24/endpoint-rule-set-1.json` & `botocore-a-la-carte-sms-1.34.9/botocore/data/sms/2016-10-24/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sms-1.34.8/botocore/data/sms/2016-10-24/paginators-1.json` & `botocore-a-la-carte-sms-1.34.9/botocore/data/sms/2016-10-24/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sms-1.34.8/botocore/data/sms/2016-10-24/service-2.json` & `botocore-a-la-carte-sms-1.34.9/botocore/data/sms/2016-10-24/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sms-1.34.8/botocore_a_la_carte_sms.egg-info/PKG-INFO` & `botocore-a-la-carte-sms-1.34.9/botocore_a_la_carte_sms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sms
-Version: 1.34.8
+Version: 1.34.9
 Summary: sms data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sms-1.34.8/setup.py` & `botocore-a-la-carte-sms-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-sms',
-    version="1.34.8",
+    version="1.34.9",
     description='sms data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/sms/*/*.json'],
```

