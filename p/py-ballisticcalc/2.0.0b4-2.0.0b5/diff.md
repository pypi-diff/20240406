# Comparing `tmp/py_ballisticcalc-2.0.0b4.tar.gz` & `tmp/py_ballisticcalc-2.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ballisticcalc-2.0.0b4.tar", last modified: Sat Apr  6 18:22:49 2024, max compression
+gzip compressed data, was "py_ballisticcalc-2.0.0b5.tar", last modified: Sat Apr  6 18:54:25 2024, max compression
```

## Comparing `py_ballisticcalc-2.0.0b4.tar` & `py_ballisticcalc-2.0.0b5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:22:49.968570 py_ballisticcalc-2.0.0b4/
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-06 18:22:49.964570 py_ballisticcalc-2.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:22:49.964570 py_ballisticcalc-2.0.0b4/py_ballisticcalc/
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/drag_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22145 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/drag_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/munition.py
--rw-r--r--   0 runner    (1001) docker     (127)    22327 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/trajectory_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/trajectory_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:22:49.964570 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-06 18:22:49.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-06 18:22:49.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:22:49.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-06 18:22:49.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 18:22:49.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:22:49.968570 py_ballisticcalc-2.0.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:22:49.964570 py_ballisticcalc-2.0.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_computer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_danger_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_mbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:54:25.350012 py_ballisticcalc-2.0.0b5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-06 18:54:25.350012 py_ballisticcalc-2.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:54:25.346012 py_ballisticcalc-2.0.0b5/py_ballisticcalc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/drag_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22145 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/drag_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/munition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22327 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/trajectory_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/trajectory_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:54:25.350012 py_ballisticcalc-2.0.0b5/py_ballisticcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-06 18:54:25.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-06 18:54:25.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:54:25.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-06 18:54:25.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 18:54:25.000000 py_ballisticcalc-2.0.0b5/py_ballisticcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:54:25.350012 py_ballisticcalc-2.0.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:54:25.350012 py_ballisticcalc-2.0.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/tests/test_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/tests/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/tests/test_computer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/tests/test_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/tests/test_danger_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/tests/test_mbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/tests/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-06 18:54:14.000000 py_ballisticcalc-2.0.0b5/tests/test_units.py
```

### Comparing `py_ballisticcalc-2.0.0b4/LICENSE` & `py_ballisticcalc-2.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/PKG-INFO` & `py_ballisticcalc-2.0.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc
-Version: 2.0.0b4
+Version: 2.0.0b5
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -186,15 +186,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: exts
-Requires-Dist: py_ballisticcalc.exts==2.0.0b4; extra == "exts"
+Requires-Dist: py_ballisticcalc.exts==2.0.0b5; extra == "exts"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Provides-Extra: charts
 Requires-Dist: matplotlib; extra == "charts"
 Requires-Dist: pandas; extra == "charts"
```

### Comparing `py_ballisticcalc-2.0.0b4/README.md` & `py_ballisticcalc-2.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/__init__.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             current_dir = parent_dir
 
     if filepath is None:
         if (filepath := find_pybc_toml()) is None:
             find_pybc_toml(os.path.dirname(__file__))
 
     logger.info(f"Found {os.path.basename(filepath)} at {os.path.dirname(filepath)}")
+    print(f"Found {os.path.basename(filepath)} at {os.path.dirname(filepath)}")
 
     with open(filepath, "rb") as fp:
         _config = tomllib.load(fp)
 
         if _pybc := _config.get('pybc'):
             if preferred_units := _pybc.get('preferred_units'):
                 PreferredUnits.set(**preferred_units)
@@ -106,14 +107,16 @@
     else:
         # trying to load definitions from pybc.toml
         _load_config(filename)
 
 
 basicConfig = _basic_config
 
+basicConfig()
+
 __all__ = [
     'Calculator',
     'basicConfig',
     'logger',
     'TrajectoryCalc',
     'get_global_max_calc_step_size',
     'get_global_use_powder_sensitivity',
```

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/backend.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/backend.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/conditions.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/conditions.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/drag_model.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/drag_model.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/drag_tables.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/drag_tables.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/example.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/example.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/interface.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/interface.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/munition.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/munition.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/trajectory_calc.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/trajectory_calc.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/trajectory_data.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/trajectory_data.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc/unit.py` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc/unit.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/PKG-INFO` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc
-Version: 2.0.0b4
+Version: 2.0.0b5
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -186,15 +186,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: exts
-Requires-Dist: py_ballisticcalc.exts==2.0.0b4; extra == "exts"
+Requires-Dist: py_ballisticcalc.exts==2.0.0b5; extra == "exts"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Provides-Extra: charts
 Requires-Dist: matplotlib; extra == "charts"
 Requires-Dist: pandas; extra == "charts"
```

### Comparing `py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/SOURCES.txt` & `py_ballisticcalc-2.0.0b5/py_ballisticcalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/pyproject.toml` & `py_ballisticcalc-2.0.0b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "py_ballisticcalc"
-version = "2.0.0b4"
+version = "2.0.0b5"
 
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
     { name="dbookstaber", email="bookstaber@gmail.com"}
 ]
 description = "LGPL library for small arms ballistic calculations (Python 3)"
 readme = "README.md"
@@ -50,10 +50,10 @@
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["py_ballisticcalc*"]  # alternatively: `exclude = ["additional*"]`
 exclude = ["py_ballisticcalc_exts*"]
 
 
 [project.optional-dependencies]
-exts = ['py_ballisticcalc.exts==2.0.0b4']
+exts = ['py_ballisticcalc.exts==2.0.0b5']
 lint = ['pylint', 'flake8']
 charts = ['matplotlib', 'pandas']
```

### Comparing `py_ballisticcalc-2.0.0b4/tests/test_atmosphere.py` & `py_ballisticcalc-2.0.0b5/tests/test_atmosphere.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/tests/test_computer.py` & `py_ballisticcalc-2.0.0b5/tests/test_computer.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/tests/test_config_loader.py` & `py_ballisticcalc-2.0.0b5/tests/test_config_loader.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/tests/test_danger_space.py` & `py_ballisticcalc-2.0.0b5/tests/test_danger_space.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/tests/test_mbc.py` & `py_ballisticcalc-2.0.0b5/tests/test_mbc.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/tests/test_trajectory.py` & `py_ballisticcalc-2.0.0b5/tests/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b4/tests/test_units.py` & `py_ballisticcalc-2.0.0b5/tests/test_units.py`

 * *Files identical despite different names*

