# Comparing `tmp/genflowly-lambda-utils-0.0.2.tar.gz` & `tmp/genflowly-lambda-utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genflowly-lambda-utils-0.0.2.tar", last modified: Wed Apr  3 03:22:30 2024, max compression
+gzip compressed data, was "genflowly-lambda-utils-0.0.3.tar", last modified: Sat Apr  6 01:07:40 2024, max compression
```

## Comparing `genflowly-lambda-utils-0.0.2.tar` & `genflowly-lambda-utils-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:22:30.924112 genflowly-lambda-utils-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-03 03:22:30.924112 genflowly-lambda-utils-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-03 03:22:04.000000 genflowly-lambda-utils-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:22:30.924112 genflowly-lambda-utils-0.0.2/genflowly_lambda_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-03 03:22:30.000000 genflowly-lambda-utils-0.0.2/genflowly_lambda_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 03:22:30.000000 genflowly-lambda-utils-0.0.2/genflowly_lambda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:22:30.000000 genflowly-lambda-utils-0.0.2/genflowly_lambda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 03:22:30.000000 genflowly-lambda-utils-0.0.2/genflowly_lambda_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 03:22:30.000000 genflowly-lambda-utils-0.0.2/genflowly_lambda_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 03:22:30.924112 genflowly-lambda-utils-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-03 03:22:04.000000 genflowly-lambda-utils-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:22:30.924112 genflowly-lambda-utils-0.0.2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:22:04.000000 genflowly-lambda-utils-0.0.2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-03 03:22:04.000000 genflowly-lambda-utils-0.0.2/utils/aws_dynamodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 03:22:04.000000 genflowly-lambda-utils-0.0.2/utils/aws_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-03 03:22:04.000000 genflowly-lambda-utils-0.0.2/utils/aws_secrets_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-03 03:22:04.000000 genflowly-lambda-utils-0.0.2/utils/aws_sns_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 03:22:04.000000 genflowly-lambda-utils-0.0.2/utils/aws_sqs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 03:22:04.000000 genflowly-lambda-utils-0.0.2/utils/aws_step_functions_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-03 03:22:04.000000 genflowly-lambda-utils-0.0.2/utils/jwt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:07:40.654190 genflowly-lambda-utils-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-06 01:07:40.654190 genflowly-lambda-utils-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:07:40.654190 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-06 01:07:40.000000 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-06 01:07:40.000000 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 01:07:40.000000 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-06 01:07:40.000000 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 01:07:40.000000 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 01:07:40.654190 genflowly-lambda-utils-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:07:40.654190 genflowly-lambda-utils-0.0.3/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_dynamodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_secrets_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_sns_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_sqs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_step_functions_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/contants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/jwt_utils.py
```

### Comparing `genflowly-lambda-utils-0.0.2/PKG-INFO` & `genflowly-lambda-utils-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.2
+Version: 0.0.3
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly-lambda-utils-0.0.2/README.md` & `genflowly-lambda-utils-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.2/genflowly_lambda_utils.egg-info/PKG-INFO` & `genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.2
+Version: 0.0.3
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly-lambda-utils-0.0.2/genflowly_lambda_utils.egg-info/requires.txt` & `genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.2/setup.py` & `genflowly-lambda-utils-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="genflowly-lambda-utils",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         "aiohttp",
         "aiosignal",
         "async-timeout",
```

### Comparing `genflowly-lambda-utils-0.0.2/utils/aws_secrets_utils.py` & `genflowly-lambda-utils-0.0.3/utils/aws_secrets_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.2/utils/aws_sns_utils.py` & `genflowly-lambda-utils-0.0.3/utils/aws_sns_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.2/utils/aws_step_functions_utils.py` & `genflowly-lambda-utils-0.0.3/utils/aws_step_functions_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.2/utils/jwt_utils.py` & `genflowly-lambda-utils-0.0.3/utils/jwt_utils.py`

 * *Files identical despite different names*

