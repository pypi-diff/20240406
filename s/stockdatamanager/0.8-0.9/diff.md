# Comparing `tmp/stockdatamanager-0.8.tar.gz` & `tmp/stockdatamanager-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockdatamanager-0.8.tar", last modified: Sat Mar 30 10:11:45 2024, max compression
+gzip compressed data, was "stockdatamanager-0.9.tar", last modified: Sat Apr  6 20:47:38 2024, max compression
```

## Comparing `stockdatamanager-0.8.tar` & `stockdatamanager-0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:11:45.083438 stockdatamanager-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-30 10:10:54.000000 stockdatamanager-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-03-30 10:11:45.083438 stockdatamanager-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-30 10:10:54.000000 stockdatamanager-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 10:11:45.083438 stockdatamanager-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-30 10:10:54.000000 stockdatamanager-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:11:45.083438 stockdatamanager-0.8/stockdatamanager/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-30 10:10:54.000000 stockdatamanager-0.8/stockdatamanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-30 10:10:54.000000 stockdatamanager-0.8/stockdatamanager/customerrors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-03-30 10:10:54.000000 stockdatamanager-0.8/stockdatamanager/datafetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-03-30 10:10:54.000000 stockdatamanager-0.8/stockdatamanager/indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)    28687 2024-03-30 10:10:54.000000 stockdatamanager-0.8/stockdatamanager/quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:11:45.083438 stockdatamanager-0.8/stockdatamanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-03-30 10:11:45.000000 stockdatamanager-0.8/stockdatamanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-30 10:11:45.000000 stockdatamanager-0.8/stockdatamanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 10:11:45.000000 stockdatamanager-0.8/stockdatamanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-30 10:11:45.000000 stockdatamanager-0.8/stockdatamanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-30 10:11:45.000000 stockdatamanager-0.8/stockdatamanager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:11:45.083438 stockdatamanager-0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-30 10:10:54.000000 stockdatamanager-0.8/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:38.853747 stockdatamanager-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 20:46:47.000000 stockdatamanager-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-06 20:47:38.853747 stockdatamanager-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-06 20:46:47.000000 stockdatamanager-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:47:38.853747 stockdatamanager-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-06 20:46:47.000000 stockdatamanager-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:38.849748 stockdatamanager-0.9/stockdatamanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/ToDo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/customerrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/datafetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56671 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:38.853747 stockdatamanager-0.9/stockdatamanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-06 20:47:38.000000 stockdatamanager-0.9/stockdatamanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 20:47:38.000000 stockdatamanager-0.9/stockdatamanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:47:38.000000 stockdatamanager-0.9/stockdatamanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-06 20:47:38.000000 stockdatamanager-0.9/stockdatamanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 20:47:38.000000 stockdatamanager-0.9/stockdatamanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:38.853747 stockdatamanager-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-06 20:46:47.000000 stockdatamanager-0.9/tests/test.py
```

### Comparing `stockdatamanager-0.8/LICENSE` & `stockdatamanager-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stockdatamanager-0.8/setup.py` & `stockdatamanager-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module sets up the package for distribution."""
 from setuptools import setup, find_packages
 
 setup(
     name='stockdatamanager',
-    version='0.8',
+    version='0.9',
     packages=find_packages(),
     description='A comprehensive library for financial analysis',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Micaletto',
     author_email='giorgio.micaletto@studbocconi.it',
     url='https://github.com/GiorgioMB/stockdatafetcher/',
```

### Comparing `stockdatamanager-0.8/stockdatamanager/datafetcher.py` & `stockdatamanager-0.9/stockdatamanager/datafetcher.py`

 * *Files identical despite different names*

### Comparing `stockdatamanager-0.8/stockdatamanager/indicators.py` & `stockdatamanager-0.9/stockdatamanager/indicators.py`

 * *Files identical despite different names*

### Comparing `stockdatamanager-0.8/tests/test.py` & `stockdatamanager-0.9/tests/test.py`

 * *Files identical despite different names*

