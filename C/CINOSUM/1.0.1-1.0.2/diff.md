# Comparing `tmp/CINOSUM-1.0.1.tar.gz` & `tmp/CINOSUM-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CINOSUM-1.0.1.tar", last modified: Sat Apr  6 02:57:50 2024, max compression
+gzip compressed data, was "CINOSUM-1.0.2.tar", last modified: Sat Apr  6 03:01:28 2024, max compression
```

## Comparing `CINOSUM-1.0.1.tar` & `CINOSUM-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 02:57:50.142093 CINOSUM-1.0.1/
-drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 02:57:50.142093 CINOSUM-1.0.1/CINOSUM.egg-info/
--rw-r--r--   0 lhy       (1003) lhy       (1003)      431 2024-04-06 02:57:50.000000 CINOSUM-1.0.1/CINOSUM.egg-info/PKG-INFO
--rw-rw-r--   0 lhy       (1003) lhy       (1003)      312 2024-04-06 02:57:50.000000 CINOSUM-1.0.1/CINOSUM.egg-info/SOURCES.txt
--rw-rw-r--   0 lhy       (1003) lhy       (1003)        1 2024-04-06 02:57:50.000000 CINOSUM-1.0.1/CINOSUM.egg-info/dependency_links.txt
--rw-rw-r--   0 lhy       (1003) lhy       (1003)       28 2024-04-06 02:57:50.000000 CINOSUM-1.0.1/CINOSUM.egg-info/requires.txt
--rw-rw-r--   0 lhy       (1003) lhy       (1003)        7 2024-04-06 02:57:50.000000 CINOSUM-1.0.1/CINOSUM.egg-info/top_level.txt
--rw-r--r--   0 lhy       (1003) lhy       (1003)      431 2024-04-06 02:57:50.142093 CINOSUM-1.0.1/PKG-INFO
-drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 02:57:50.142093 CINOSUM-1.0.1/models/
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     4519 2024-04-04 04:13:54.000000 CINOSUM-1.0.1/models/CINOSUM.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)        0 2024-03-26 02:05:37.000000 CINOSUM-1.0.1/models/__init__.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     4826 2024-04-04 01:47:17.000000 CINOSUM-1.0.1/models/encoder.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)    12903 2024-04-04 03:41:49.000000 CINOSUM-1.0.1/models/generate.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     3963 2024-03-27 01:19:12.000000 CINOSUM-1.0.1/models/model_builder.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     8340 2024-03-26 02:05:37.000000 CINOSUM-1.0.1/models/neural.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     9649 2024-03-26 02:05:37.000000 CINOSUM-1.0.1/models/optimizers.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     3886 2024-04-01 13:19:09.000000 CINOSUM-1.0.1/models/rnn.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)       38 2024-04-06 02:57:50.142093 CINOSUM-1.0.1/setup.cfg
--rw-rw-r--   0 lhy       (1003) lhy       (1003)      578 2024-04-06 02:57:30.000000 CINOSUM-1.0.1/setup.py
+drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:01:28.794221 CINOSUM-1.0.2/
+drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:01:28.794221 CINOSUM-1.0.2/CINOSUM/
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     4519 2024-04-04 04:13:54.000000 CINOSUM-1.0.2/CINOSUM/CINOSUM.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)        0 2024-03-26 02:05:37.000000 CINOSUM-1.0.2/CINOSUM/__init__.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     4826 2024-04-04 01:47:17.000000 CINOSUM-1.0.2/CINOSUM/encoder.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)    12903 2024-04-04 03:41:49.000000 CINOSUM-1.0.2/CINOSUM/generate.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     3963 2024-03-27 01:19:12.000000 CINOSUM-1.0.2/CINOSUM/model_builder.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     8340 2024-03-26 02:05:37.000000 CINOSUM-1.0.2/CINOSUM/neural.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     9649 2024-03-26 02:05:37.000000 CINOSUM-1.0.2/CINOSUM/optimizers.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     3886 2024-04-01 13:19:09.000000 CINOSUM-1.0.2/CINOSUM/rnn.py
+drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:01:28.794221 CINOSUM-1.0.2/CINOSUM.egg-info/
+-rw-r--r--   0 lhy       (1003) lhy       (1003)      431 2024-04-06 03:01:28.000000 CINOSUM-1.0.2/CINOSUM.egg-info/PKG-INFO
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)      320 2024-04-06 03:01:28.000000 CINOSUM-1.0.2/CINOSUM.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)        1 2024-04-06 03:01:28.000000 CINOSUM-1.0.2/CINOSUM.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)       28 2024-04-06 03:01:28.000000 CINOSUM-1.0.2/CINOSUM.egg-info/requires.txt
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)        8 2024-04-06 03:01:28.000000 CINOSUM-1.0.2/CINOSUM.egg-info/top_level.txt
+-rw-r--r--   0 lhy       (1003) lhy       (1003)      431 2024-04-06 03:01:28.794221 CINOSUM-1.0.2/PKG-INFO
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)       38 2024-04-06 03:01:28.794221 CINOSUM-1.0.2/setup.cfg
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)      578 2024-04-06 03:01:26.000000 CINOSUM-1.0.2/setup.py
```

### Comparing `CINOSUM-1.0.1/models/CINOSUM.py` & `CINOSUM-1.0.2/CINOSUM/CINOSUM.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.1/models/encoder.py` & `CINOSUM-1.0.2/CINOSUM/encoder.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.1/models/generate.py` & `CINOSUM-1.0.2/CINOSUM/generate.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.1/models/model_builder.py` & `CINOSUM-1.0.2/CINOSUM/model_builder.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.1/models/neural.py` & `CINOSUM-1.0.2/CINOSUM/neural.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.1/models/optimizers.py` & `CINOSUM-1.0.2/CINOSUM/optimizers.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.1/models/rnn.py` & `CINOSUM-1.0.2/CINOSUM/rnn.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.1/setup.py` & `CINOSUM-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CINOSUM',
-    version='1.0.1',
+    version='1.0.2',
     description='Chinese Minority Extractive Multi-language summarization project',
     author='HaoYu Luo',
     author_email='506685820@qq.com',
     packages=find_packages(),
     install_requires=[
         'torch',
         'numpy',
```

