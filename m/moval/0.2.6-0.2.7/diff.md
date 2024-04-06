# Comparing `tmp/moval-0.2.6.tar.gz` & `tmp/moval-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-4by5kalk/moval-0.2.6.tar", last modified: Thu Mar 21 04:43:10 2024, max compression
+gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-40zndkpl/moval-0.2.7.tar", last modified: Sat Apr  6 17:45:30 2024, max compression
```

## Comparing `moval-0.2.6.tar` & `moval-0.2.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-03-21 04:43:10.329702 moval-0.2.6/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-03-21 04:43:10.329625 moval-0.2.6/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.2.6/README.md
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-03-21 04:43:10.323461 moval-0.2.6/moval/
--rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-03-21 04:41:04.000000 moval-0.2.6/moval/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-03-21 04:43:10.324687 moval-0.2.6/moval/integrations/
--rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.2.6/moval/integrations/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-03-21 04:43:10.325300 moval-0.2.6/moval/integrations/sklearn/
--rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.2.6/moval/integrations/sklearn/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    41022 2024-03-21 04:23:11.000000 moval-0.2.6/moval/integrations/sklearn/moval.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-03-21 04:43:10.327629 moval-0.2.6/moval/models/
--rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.2.6/moval/models/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.2.6/moval/models/confidences.py
--rw-r--r--   0 zejuli     (501) staff       (20)    45579 2024-03-21 04:07:43.000000 moval-0.2.6/moval/models/model.py
--rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.2.6/moval/models/solver_temperature.py
--rw-r--r--   0 zejuli     (501) staff       (20)    10516 2024-01-15 18:30:37.000000 moval-0.2.6/moval/models/utils.py
--rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.2.6/moval/registry.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-03-21 04:43:10.328973 moval-0.2.6/moval/solvers/
--rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.2.6/moval/solvers/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    12101 2024-03-21 04:27:22.000000 moval-0.2.6/moval/solvers/criterions.py
--rw-r--r--   0 zejuli     (501) staff       (20)    19432 2024-03-21 04:39:11.000000 moval-0.2.6/moval/solvers/solver.py
--rw-r--r--   0 zejuli     (501) staff       (20)     2807 2024-03-21 04:25:50.000000 moval-0.2.6/moval/solvers/utils.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-03-21 04:43:10.329352 moval-0.2.6/moval.egg-info/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-03-21 04:43:10.000000 moval-0.2.6/moval.egg-info/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-03-21 04:43:10.000000 moval-0.2.6/moval.egg-info/SOURCES.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-03-21 04:43:10.000000 moval-0.2.6/moval.egg-info/dependency_links.txt
--rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-03-21 04:43:10.000000 moval-0.2.6/moval.egg-info/requires.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-03-21 04:43:10.000000 moval-0.2.6/moval.egg-info/top_level.txt
--rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.2.6/pyproject.toml
--rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-03-21 04:43:10.330081 moval-0.2.6/setup.cfg
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 17:45:30.583660 moval-0.2.7/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-06 17:45:30.583603 moval-0.2.7/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.2.7/README.md
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 17:45:30.580311 moval-0.2.7/moval/
+-rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-04-06 17:44:44.000000 moval-0.2.7/moval/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 17:45:30.581306 moval-0.2.7/moval/integrations/
+-rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.2.7/moval/integrations/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 17:45:30.581603 moval-0.2.7/moval/integrations/sklearn/
+-rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.2.7/moval/integrations/sklearn/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    41022 2024-03-21 04:23:11.000000 moval-0.2.7/moval/integrations/sklearn/moval.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 17:45:30.582529 moval-0.2.7/moval/models/
+-rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.2.7/moval/models/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.2.7/moval/models/confidences.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    45579 2024-03-21 04:07:43.000000 moval-0.2.7/moval/models/model.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.2.7/moval/models/solver_temperature.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    10516 2024-01-15 18:30:37.000000 moval-0.2.7/moval/models/utils.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.2.7/moval/registry.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 17:45:30.583193 moval-0.2.7/moval/solvers/
+-rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.2.7/moval/solvers/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    12103 2024-04-06 17:43:16.000000 moval-0.2.7/moval/solvers/criterions.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    19432 2024-03-21 04:39:11.000000 moval-0.2.7/moval/solvers/solver.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     2807 2024-03-21 04:25:50.000000 moval-0.2.7/moval/solvers/utils.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 17:45:30.583383 moval-0.2.7/moval.egg-info/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-06 17:45:30.000000 moval-0.2.7/moval.egg-info/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-04-06 17:45:30.000000 moval-0.2.7/moval.egg-info/SOURCES.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-04-06 17:45:30.000000 moval-0.2.7/moval.egg-info/dependency_links.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-04-06 17:45:30.000000 moval-0.2.7/moval.egg-info/requires.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-04-06 17:45:30.000000 moval-0.2.7/moval.egg-info/top_level.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.2.7/pyproject.toml
+-rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-04-06 17:45:30.583985 moval-0.2.7/setup.cfg
```

### Comparing `moval-0.2.6/PKG-INFO` & `moval-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.2.6
+Version: 0.2.7
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.2.6 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.2.7 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.2.6/README.md` & `moval-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/moval/__init__.py` & `moval-0.2.7/moval/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     from moval.integrations.sklearn.moval import MOVAL
 except ImportError as e:
     # silently fail for now
     pass
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __all__ = ["MOVAL"]
 
 def __getattr__(key):
     """Lazy import of moval submodules and -packages.
 
     Once :py:mod:`moval` is imported, it is possible to lazy import
```

### Comparing `moval-0.2.6/moval/integrations/sklearn/moval.py` & `moval-0.2.7/moval/integrations/sklearn/moval.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/moval/models/confidences.py` & `moval-0.2.7/moval/models/confidences.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/moval/models/model.py` & `moval-0.2.7/moval/models/model.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/moval/models/solver_temperature.py` & `moval-0.2.7/moval/models/solver_temperature.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/moval/models/utils.py` & `moval-0.2.7/moval/models/utils.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/moval/registry.py` & `moval-0.2.7/moval/registry.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/moval/solvers/criterions.py` & `moval-0.2.7/moval/solvers/criterions.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
         else:
 
             err = np.zeros(inp.shape[1])
 
             if self.metric == "accuracy":
                 for kcls in range(inp.shape[1]):
-                    pos_cls = np.where(gt == kcls)[0]
+                    pos_cls = np.where(pred == kcls)[0]
                     acc_cls = np.sum(gt[pos_cls] == pred[pos_cls]) / len(gt[pos_cls])
 
                     err[kcls] = estim[kcls] - acc_cls
 
             elif self.metric == "sensitivity":
                 sensitivities = []
                 for kcls in range(inp.shape[1]):
```

### Comparing `moval-0.2.6/moval/solvers/solver.py` & `moval-0.2.7/moval/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/moval/solvers/utils.py` & `moval-0.2.7/moval/solvers/utils.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/moval.egg-info/PKG-INFO` & `moval-0.2.7/moval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.2.6
+Version: 0.2.7
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.2.6 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.2.7 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.2.6/moval.egg-info/SOURCES.txt` & `moval-0.2.7/moval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/pyproject.toml` & `moval-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moval-0.2.6/setup.cfg` & `moval-0.2.7/setup.cfg`

 * *Files identical despite different names*

