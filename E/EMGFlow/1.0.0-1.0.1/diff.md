# Comparing `tmp/emgflow-1.0.0.tar.gz` & `tmp/emgflow-1.0.1.tar.gz`

## Comparing `emgflow-1.0.0.tar` & `emgflow-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 emgflow-1.0.0/src/EMGFlow/OutlierFinder.py
--rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 emgflow-1.0.0/src/EMGFlow/PlotSignals.py
--rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.0/src/EMGFlow/SignalFilterer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.0/src/EMGFlow/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.0/.gitignore
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 emgflow-1.0.0/README.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 emgflow-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 emgflow-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 emgflow-1.0.1/src/EMGFlow/OutlierFinder.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 emgflow-1.0.1/src/EMGFlow/PlotSignals.py
+-rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.1/src/EMGFlow/SignalFilterer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.1/src/EMGFlow/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.1/.gitignore
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 emgflow-1.0.1/README.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 emgflow-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 emgflow-1.0.1/PKG-INFO
```

### Comparing `emgflow-1.0.0/src/EMGFlow/OutlierFinder.py` & `emgflow-1.0.1/src/EMGFlow/OutlierFinder.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.0/src/EMGFlow/PlotSignals.py` & `emgflow-1.0.1/src/EMGFlow/PlotSignals.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.0/src/EMGFlow/SignalFilterer.py` & `emgflow-1.0.1/src/EMGFlow/SignalFilterer.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.0/pyproject.toml` & `emgflow-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EMGFlow"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = [
     "pandas",
     "numpy",
     "scipy",
     "matplotlib",
     "opencv-python", 
     "tqdm"
```

