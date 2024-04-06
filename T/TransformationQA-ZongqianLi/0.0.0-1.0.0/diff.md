# Comparing `tmp/TransformationQA_ZongqianLi-0.0.0.tar.gz` & `tmp/TransformationQA_ZongqianLi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TransformationQA_ZongqianLi-0.0.0.tar", last modified: Sat Apr  6 13:50:37 2024, max compression
+gzip compressed data, was "TransformationQA_ZongqianLi-1.0.0.tar", last modified: Sat Apr  6 13:55:28 2024, max compression
```

## Comparing `TransformationQA_ZongqianLi-0.0.0.tar` & `TransformationQA_ZongqianLi-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwsr-x   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:50:37.000000 TransformationQA_ZongqianLi-0.0.0/
--rw-rw-r--   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:48:14.000000 TransformationQA_ZongqianLi-0.0.0/LICENSE
--rw-r--r--   0 zl510    (45969) zl510    (45979)       93 2024-04-06 13:50:37.000000 TransformationQA_ZongqianLi-0.0.0/PKG-INFO
--rw-rw-r--   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:47:52.000000 TransformationQA_ZongqianLi-0.0.0/README.md
--rw-rw-r--   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:44:54.000000 TransformationQA_ZongqianLi-0.0.0/pyproject.toml
--rw-rw-r--   0 zl510    (45969) zl510    (45979)       38 2024-04-06 13:50:37.000000 TransformationQA_ZongqianLi-0.0.0/setup.cfg
-drwxrwsr-x   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:50:37.000000 TransformationQA_ZongqianLi-0.0.0/src/
-drwxrwsr-x   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:50:37.000000 TransformationQA_ZongqianLi-0.0.0/src/TransformationQA_ZongqianLi/
--rw-rw-r--   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:48:51.000000 TransformationQA_ZongqianLi-0.0.0/src/TransformationQA_ZongqianLi/__init__.py
--rw-rw-r--   0 zl510    (45969) zl510    (45979)    21956 2024-04-06 13:49:02.000000 TransformationQA_ZongqianLi-0.0.0/src/TransformationQA_ZongqianLi/transformationqa.py
-drwxrwsr-x   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:50:37.000000 TransformationQA_ZongqianLi-0.0.0/src/TransformationQA_ZongqianLi.egg-info/
--rw-r--r--   0 zl510    (45969) zl510    (45979)       93 2024-04-06 13:50:37.000000 TransformationQA_ZongqianLi-0.0.0/src/TransformationQA_ZongqianLi.egg-info/PKG-INFO
--rw-rw-r--   0 zl510    (45969) zl510    (45979)      348 2024-04-06 13:50:37.000000 TransformationQA_ZongqianLi-0.0.0/src/TransformationQA_ZongqianLi.egg-info/SOURCES.txt
--rw-rw-r--   0 zl510    (45969) zl510    (45979)        1 2024-04-06 13:50:37.000000 TransformationQA_ZongqianLi-0.0.0/src/TransformationQA_ZongqianLi.egg-info/dependency_links.txt
--rw-rw-r--   0 zl510    (45969) zl510    (45979)       28 2024-04-06 13:50:37.000000 TransformationQA_ZongqianLi-0.0.0/src/TransformationQA_ZongqianLi.egg-info/top_level.txt
+drwxrwsr-x   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:55:28.000000 TransformationQA_ZongqianLi-1.0.0/
+-rw-rw-r--   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:48:14.000000 TransformationQA_ZongqianLi-1.0.0/LICENSE
+-rw-r--r--   0 zl510    (45969) zl510    (45979)      567 2024-04-06 13:55:28.000000 TransformationQA_ZongqianLi-1.0.0/PKG-INFO
+-rw-rw-r--   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:47:52.000000 TransformationQA_ZongqianLi-1.0.0/README.md
+-rw-rw-r--   0 zl510    (45969) zl510    (45979)      682 2024-04-06 13:55:20.000000 TransformationQA_ZongqianLi-1.0.0/pyproject.toml
+-rw-rw-r--   0 zl510    (45969) zl510    (45979)       38 2024-04-06 13:55:28.000000 TransformationQA_ZongqianLi-1.0.0/setup.cfg
+drwxrwsr-x   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:55:28.000000 TransformationQA_ZongqianLi-1.0.0/src/
+drwxrwsr-x   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:55:28.000000 TransformationQA_ZongqianLi-1.0.0/src/TransformationQA_ZongqianLi/
+-rw-rw-r--   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:48:51.000000 TransformationQA_ZongqianLi-1.0.0/src/TransformationQA_ZongqianLi/__init__.py
+-rw-rw-r--   0 zl510    (45969) zl510    (45979)    21956 2024-04-06 13:49:02.000000 TransformationQA_ZongqianLi-1.0.0/src/TransformationQA_ZongqianLi/transformation.py
+drwxrwsr-x   0 zl510    (45969) zl510    (45979)        0 2024-04-06 13:55:28.000000 TransformationQA_ZongqianLi-1.0.0/src/TransformationQA_ZongqianLi.egg-info/
+-rw-r--r--   0 zl510    (45969) zl510    (45979)      567 2024-04-06 13:55:28.000000 TransformationQA_ZongqianLi-1.0.0/src/TransformationQA_ZongqianLi.egg-info/PKG-INFO
+-rw-rw-r--   0 zl510    (45969) zl510    (45979)      346 2024-04-06 13:55:28.000000 TransformationQA_ZongqianLi-1.0.0/src/TransformationQA_ZongqianLi.egg-info/SOURCES.txt
+-rw-rw-r--   0 zl510    (45969) zl510    (45979)        1 2024-04-06 13:55:28.000000 TransformationQA_ZongqianLi-1.0.0/src/TransformationQA_ZongqianLi.egg-info/dependency_links.txt
+-rw-rw-r--   0 zl510    (45969) zl510    (45979)       28 2024-04-06 13:55:28.000000 TransformationQA_ZongqianLi-1.0.0/src/TransformationQA_ZongqianLi.egg-info/top_level.txt
```

### Comparing `TransformationQA_ZongqianLi-0.0.0/src/TransformationQA_ZongqianLi/transformationqa.py` & `TransformationQA_ZongqianLi-1.0.0/src/TransformationQA_ZongqianLi/transformation.py`

 * *Files identical despite different names*

