# Comparing `tmp/wolta-0.1.5.tar.gz` & `tmp/wolta-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolta-0.1.5.tar", last modified: Sat Apr  6 14:10:07 2024, max compression
+gzip compressed data, was "wolta-0.1.6.tar", last modified: Sat Apr  6 14:27:29 2024, max compression
```

## Comparing `wolta-0.1.5.tar` & `wolta-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 14:10:07.134748 wolta-0.1.5/
--rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0    15098 2024-04-06 14:10:07.133705 wolta-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    13874 2024-04-02 23:36:26.000000 wolta-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 14:10:07.134748 wolta-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1209 2024-04-06 14:09:26.000000 wolta-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 14:10:07.077136 wolta-0.1.5/wolta/
--rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.5/wolta/__init__.py
--rw-rw-rw-   0        0        0     7849 2024-04-06 14:08:07.000000 wolta-0.1.5/wolta/data_tools.py
--rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.5/wolta/feature_tools.py
--rw-rw-rw-   0        0        0    18051 2024-04-06 14:08:07.000000 wolta-0.1.5/wolta/model_tools.py
--rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.5/wolta/progressive_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-06 14:10:07.131472 wolta-0.1.5/wolta.egg-info/
--rw-rw-rw-   0        0        0    15098 2024-04-06 14:10:06.000000 wolta-0.1.5/wolta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-06 14:10:06.000000 wolta-0.1.5/wolta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 14:10:06.000000 wolta-0.1.5/wolta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-06 14:10:06.000000 wolta-0.1.5/wolta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       61 2024-04-06 14:10:06.000000 wolta-0.1.5/wolta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 14:27:29.205649 wolta-0.1.6/
+-rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0    15098 2024-04-06 14:27:29.205649 wolta-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    13874 2024-04-02 23:36:26.000000 wolta-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 14:27:29.205649 wolta-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2024-04-06 14:27:24.000000 wolta-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:27:29.189380 wolta-0.1.6/wolta/
+-rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.6/wolta/__init__.py
+-rw-rw-rw-   0        0        0     7843 2024-04-06 14:27:03.000000 wolta-0.1.6/wolta/data_tools.py
+-rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.6/wolta/feature_tools.py
+-rw-rw-rw-   0        0        0    18051 2024-04-06 14:08:07.000000 wolta-0.1.6/wolta/model_tools.py
+-rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.6/wolta/progressive_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:27:29.204623 wolta-0.1.6/wolta.egg-info/
+-rw-rw-rw-   0        0        0    15098 2024-04-06 14:27:29.000000 wolta-0.1.6/wolta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-06 14:27:29.000000 wolta-0.1.6/wolta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 14:27:29.000000 wolta-0.1.6/wolta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-06 14:27:29.000000 wolta-0.1.6/wolta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       61 2024-04-06 14:27:29.000000 wolta-0.1.6/wolta.egg-info/top_level.txt
```

### Comparing `wolta-0.1.5/LICENSE.txt` & `wolta-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wolta-0.1.5/PKG-INFO` & `wolta-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.5
+Version: 0.1.6
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wolta-0.1.5/README.md` & `wolta-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `wolta-0.1.5/setup.py` & `wolta-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Data Science Library'
 LONG_DESCRIPTION = 'A package for data science'
 
 setup(
     name="wolta",
     version=VERSION,
     author="iamalreadynoob",
```

### Comparing `wolta-0.1.5/wolta/data_tools.py` & `wolta-0.1.6/wolta/data_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 
             if print_description:
                 print('part {} is done'.format(str(part)))
 
             part += 1
 
 
-def make_normal(self, X, y, strategy='log'):
+def make_normal(X, y, strategy='log'):
     import numpy as np
 
     if strategy == 'log':
         X = np.log(X + 1)
         y = np.log(y + 1)
 
         return X, y
```

### Comparing `wolta-0.1.5/wolta/feature_tools.py` & `wolta-0.1.6/wolta/feature_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.5/wolta/model_tools.py` & `wolta-0.1.6/wolta/model_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.5/wolta/progressive_tools.py` & `wolta-0.1.6/wolta/progressive_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.5/wolta.egg-info/PKG-INFO` & `wolta-0.1.6/wolta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.5
+Version: 0.1.6
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

