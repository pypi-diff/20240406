# Comparing `tmp/wolta-0.1.4.tar.gz` & `tmp/wolta-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolta-0.1.4.tar", last modified: Tue Apr  2 23:38:13 2024, max compression
+gzip compressed data, was "wolta-0.1.5.tar", last modified: Sat Apr  6 14:10:07 2024, max compression
```

## Comparing `wolta-0.1.4.tar` & `wolta-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 23:38:13.514831 wolta-0.1.4/
--rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0    15048 2024-04-02 23:38:13.514688 wolta-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    13874 2024-04-02 23:36:26.000000 wolta-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 23:38:13.515853 wolta-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1185 2024-04-02 23:37:26.000000 wolta-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:38:13.464742 wolta-0.1.4/wolta/
--rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.4/wolta/__init__.py
--rw-rw-rw-   0        0        0     7564 2024-04-01 19:35:23.000000 wolta-0.1.4/wolta/data_tools.py
--rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.4/wolta/feature_tools.py
--rw-rw-rw-   0        0        0     8993 2024-04-02 23:24:20.000000 wolta-0.1.4/wolta/model_tools.py
--rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.4/wolta/progressive_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:38:13.512570 wolta-0.1.4/wolta.egg-info/
--rw-rw-rw-   0        0        0    15048 2024-04-02 23:38:13.000000 wolta-0.1.4/wolta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-02 23:38:13.000000 wolta-0.1.4/wolta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 23:38:13.000000 wolta-0.1.4/wolta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-02 23:38:13.000000 wolta-0.1.4/wolta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       61 2024-04-02 23:38:13.000000 wolta-0.1.4/wolta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 14:10:07.134748 wolta-0.1.5/
+-rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    15098 2024-04-06 14:10:07.133705 wolta-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13874 2024-04-02 23:36:26.000000 wolta-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 14:10:07.134748 wolta-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2024-04-06 14:09:26.000000 wolta-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:10:07.077136 wolta-0.1.5/wolta/
+-rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.5/wolta/__init__.py
+-rw-rw-rw-   0        0        0     7849 2024-04-06 14:08:07.000000 wolta-0.1.5/wolta/data_tools.py
+-rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.5/wolta/feature_tools.py
+-rw-rw-rw-   0        0        0    18051 2024-04-06 14:08:07.000000 wolta-0.1.5/wolta/model_tools.py
+-rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.5/wolta/progressive_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:10:07.131472 wolta-0.1.5/wolta.egg-info/
+-rw-rw-rw-   0        0        0    15098 2024-04-06 14:10:06.000000 wolta-0.1.5/wolta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-06 14:10:06.000000 wolta-0.1.5/wolta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 14:10:06.000000 wolta-0.1.5/wolta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-06 14:10:06.000000 wolta-0.1.5/wolta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       61 2024-04-06 14:10:06.000000 wolta-0.1.5/wolta.egg-info/top_level.txt
```

### Comparing `wolta-0.1.4/LICENSE.txt` & `wolta-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wolta-0.1.4/PKG-INFO` & `wolta-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.4
+Version: 0.1.5
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,16 @@
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: hyperopt
+Requires-Dist: catboost
+Requires-Dist: imblearn
 
 
 # WOLTA DOCUMENTATION
 
 Wolta is designed for making simplify the frequently used processes which includes Pandas, Numpy and Scikit-Learn in Machine Learning.
 <br><br>
 Currently there are four modules inside the library, which are 'data_tools', 'model_tools', 'progressive_tools' and 'feature_tools'
```

### Comparing `wolta-0.1.4/README.md` & `wolta-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `wolta-0.1.4/setup.py` & `wolta-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'Data Science Library'
 LONG_DESCRIPTION = 'A package for data science'
 
 setup(
     name="wolta",
     version=VERSION,
     author="iamalreadynoob",
     author_email="<sadikefe69@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['scikit-learn', 'pandas', 'numpy', 'hyperopt'],
+    install_requires=['scikit-learn', 'pandas', 'numpy', 'hyperopt', 'catboost', 'imblearn'],
     keywords=['python', 'machine', 'learning', 'machine learning', 'data science', 'data'],
     py_modules=['data_tools', 'model_tools', 'progressive_tools', 'feature_tools'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

### Comparing `wolta-0.1.4/wolta/data_tools.py` & `wolta-0.1.5/wolta/data_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,8 +277,24 @@
 
             with open(sub_path, 'w', newline='') as sf:
                 sf.writelines(sub)
 
             if print_description:
                 print('part {} is done'.format(str(part)))
 
-            part += 1
+            part += 1
+
+
+def make_normal(self, X, y, strategy='log'):
+    import numpy as np
+
+    if strategy == 'log':
+        X = np.log(X + 1)
+        y = np.log(y + 1)
+
+        return X, y
+
+    elif strategy == 'sqrt':
+        X = np.sqrt(X)
+        y = np.sqrt(y)
+
+        return X, y
```

### Comparing `wolta-0.1.4/wolta/feature_tools.py` & `wolta-0.1.5/wolta/feature_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.4/wolta/progressive_tools.py` & `wolta-0.1.5/wolta/progressive_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.4/wolta.egg-info/PKG-INFO` & `wolta-0.1.5/wolta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.4
+Version: 0.1.5
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,16 @@
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: hyperopt
+Requires-Dist: catboost
+Requires-Dist: imblearn
 
 
 # WOLTA DOCUMENTATION
 
 Wolta is designed for making simplify the frequently used processes which includes Pandas, Numpy and Scikit-Learn in Machine Learning.
 <br><br>
 Currently there are four modules inside the library, which are 'data_tools', 'model_tools', 'progressive_tools' and 'feature_tools'
```

