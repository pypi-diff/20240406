# Comparing `tmp/dstool-0.1.0.tar.gz` & `tmp/dstool-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstool-0.1.0.tar", last modified: Mon Apr  1 14:52:28 2024, max compression
+gzip compressed data, was "dstool-0.1.0a0.tar", last modified: Sat Apr  6 17:55:02 2024, max compression
```

## Comparing `dstool-0.1.0.tar` & `dstool-0.1.0a0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.112434 dstool-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 14:52:15.000000 dstool-0.1.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-01 14:52:15.000000 dstool-0.1.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 14:52:15.000000 dstool-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-01 14:52:15.000000 dstool-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-01 14:52:28.112434 dstool-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-01 14:52:15.000000 dstool-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.104434 dstool-0.1.0/dstool/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.108434 dstool-0.1.0/dstool/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/decorators/class_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/decorators/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/decorators/measure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.108434 dstool-0.1.0/dstool/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/parallel/parallel_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.108434 dstool-0.1.0/dstool/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/plot/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.108434 dstool-0.1.0/dstool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:52:28.112434 dstool-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-01 14:52:15.000000 dstool-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.108434 dstool-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:15.000000 dstool-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-01 14:52:15.000000 dstool-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 14:52:15.000000 dstool-0.1.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:02.727329 dstool-0.1.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 17:54:54.000000 dstool-0.1.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-06 17:54:54.000000 dstool-0.1.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-06 17:55:02.727329 dstool-0.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-06 17:54:54.000000 dstool-0.1.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:02.723329 dstool-0.1.0a0/dstool/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:02.723329 dstool-0.1.0a0/dstool/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/decorators/class_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/decorators/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/decorators/measure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:02.723329 dstool-0.1.0a0/dstool/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/parallel/parallel_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:02.723329 dstool-0.1.0a0/dstool/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/plot/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:02.723329 dstool-0.1.0a0/dstool/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 17:54:54.000000 dstool-0.1.0a0/dstool/tensors/safetensors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:02.727329 dstool-0.1.0a0/dstool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-06 17:55:02.000000 dstool-0.1.0a0/dstool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-06 17:55:02.000000 dstool-0.1.0a0/dstool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:55:02.000000 dstool-0.1.0a0/dstool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 17:55:02.000000 dstool-0.1.0a0/dstool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-06 17:55:02.000000 dstool-0.1.0a0/dstool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 17:55:02.000000 dstool-0.1.0a0/dstool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 17:55:02.727329 dstool-0.1.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-06 17:54:54.000000 dstool-0.1.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:02.723329 dstool-0.1.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:54:54.000000 dstool-0.1.0a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-06 17:54:54.000000 dstool-0.1.0a0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 17:54:54.000000 dstool-0.1.0a0/tests/test_base.py
```

### Comparing `dstool-0.1.0/LICENSE` & `dstool-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dstool-0.1.0/PKG-INFO` & `dstool-0.1.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: dstool
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: Awesome dstool created by xzyaoi
 Home-page: https://github.com/xzyaoi/dstool/
 Author: xzyaoi
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: plotly
+Requires-Dist: rich
+Requires-Dist: safetensors
+Requires-Dist: typer
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `dstool-0.1.0/README.md` & `dstool-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `dstool-0.1.0/dstool/decorators/debugger.py` & `dstool-0.1.0a0/dstool/decorators/debugger.py`

 * *Files identical despite different names*

### Comparing `dstool-0.1.0/dstool/decorators/measure.py` & `dstool-0.1.0a0/dstool/decorators/measure.py`

 * *Files identical despite different names*

### Comparing `dstool-0.1.0/dstool/parallel/parallel_func.py` & `dstool-0.1.0a0/dstool/parallel/parallel_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from multiprocessing import cpu_count
 from typing import Callable
-
 from joblib import Parallel, delayed
 
 
 def parallel(
     func=None, args=(), merge_func=lambda x: x, parallelism=cpu_count()
 ):
```

### Comparing `dstool-0.1.0/dstool/plot/style.py` & `dstool-0.1.0a0/dstool/plot/style.py`

 * *Files identical despite different names*

### Comparing `dstool-0.1.0/dstool.egg-info/PKG-INFO` & `dstool-0.1.0a0/dstool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: dstool
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: Awesome dstool created by xzyaoi
 Home-page: https://github.com/xzyaoi/dstool/
 Author: xzyaoi
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: plotly
+Requires-Dist: rich
+Requires-Dist: safetensors
+Requires-Dist: typer
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `dstool-0.1.0/dstool.egg-info/SOURCES.txt` & `dstool-0.1.0a0/dstool.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-Containerfile
-HISTORY.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 dstool/VERSION
 dstool/__init__.py
 dstool/__main__.py
 dstool/base.py
-dstool/cli.py
 dstool.egg-info/PKG-INFO
 dstool.egg-info/SOURCES.txt
 dstool.egg-info/dependency_links.txt
 dstool.egg-info/entry_points.txt
 dstool.egg-info/requires.txt
 dstool.egg-info/top_level.txt
 dstool/decorators/__init__.py
 dstool/decorators/class_utils.py
 dstool/decorators/debugger.py
 dstool/decorators/measure.py
 dstool/parallel/__init__.py
 dstool/parallel/parallel_func.py
 dstool/plot/style.py
+dstool/tensors/safetensors.py
 tests/__init__.py
 tests/conftest.py
 tests/test_base.py
```

### Comparing `dstool-0.1.0/setup.py` & `dstool-0.1.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,11 +36,11 @@
     url="https://github.com/xzyaoi/dstool/",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="xzyaoi",
     packages=find_packages(exclude=["tests", ".github"]),
     install_requires=read_requirements("requirements.txt"),
     entry_points={
-        "console_scripts": ["dstool = dstool.__main__:main"]
+        "dstool": ["dstool = dstool.__main__:main"]
     },
     extras_require={"test": read_requirements("requirements-test.txt")},
 )
```

