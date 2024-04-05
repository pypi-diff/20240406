# Comparing `tmp/PH-Baseliner-1.3.1.tar.gz` & `tmp/PH-Baseliner-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-Baseliner-1.3.1.tar", last modified: Sun Nov 12 18:29:59 2023, max compression
+gzip compressed data, was "PH-Baseliner-1.3.2.tar", last modified: Fri Apr  5 22:52:53 2024, max compression
```

## Comparing `PH-Baseliner-1.3.1.tar` & `PH-Baseliner-1.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2023-11-12 18:27:30.000000 PH-Baseliner-1.3.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35149 2023-11-12 18:27:30.000000 PH-Baseliner-1.3.1/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/PH_Baseliner.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2588 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/PH_Baseliner.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      762 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/PH_Baseliner.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/PH_Baseliner.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/PH_Baseliner.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2588 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1589 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/README.md
--rw-r--r--   0 runner     (501) staff       (20)       44 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/ph_baseliner/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/ph_baseliner/codes/
--rw-r--r--   0 runner     (501) staff       (20)    13031 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/codes/ECCCNYS_2020.json
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/codes/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2072 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/codes/lighting_space_types.py
--rw-r--r--   0 runner     (501) staff       (20)    17467 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/codes/model.py
--rw-r--r--   0 runner     (501) staff       (20)     1406 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/codes/options.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/ph_baseliner/phpp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phpp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4691 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phpp/areas.py
--rw-r--r--   0 runner     (501) staff       (20)     1484 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phpp/components.py
--rw-r--r--   0 runner     (501) staff       (20)     2510 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phpp/lighting.py
--rw-r--r--   0 runner     (501) staff       (20)     3285 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phpp/u_values.py
--rw-r--r--   0 runner     (501) staff       (20)     5618 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phpp/windows.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/ph_baseliner/phx/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phx/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2526 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phx/areas.py
--rw-r--r--   0 runner     (501) staff       (20)     2583 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phx/constructions.py
--rw-r--r--   0 runner     (501) staff       (20)      488 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phx/lighting.py
--rw-r--r--   0 runner     (501) staff       (20)     7637 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/ph_baseliner/phx/windows.py
--rw-r--r--   0 runner     (501) staff       (20)       87 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)      839 2023-11-12 18:29:59.000000 PH-Baseliner-1.3.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-11-12 18:27:31.000000 PH-Baseliner-1.3.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:53.347401 PH-Baseliner-1.3.2/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:53.338440 PH-Baseliner-1.3.2/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:53.341116 PH-Baseliner-1.3.2/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1875 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35149 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:53.342272 PH-Baseliner-1.3.2/PH_Baseliner.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2258 2024-04-05 22:52:53.000000 PH-Baseliner-1.3.2/PH_Baseliner.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      762 2024-04-05 22:52:53.000000 PH-Baseliner-1.3.2/PH_Baseliner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-05 22:52:53.000000 PH-Baseliner-1.3.2/PH_Baseliner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       13 2024-04-05 22:52:53.000000 PH-Baseliner-1.3.2/PH_Baseliner.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2258 2024-04-05 22:52:53.347565 PH-Baseliner-1.3.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       44 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:53.342541 PH-Baseliner-1.3.2/ph_baseliner/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:53.343973 PH-Baseliner-1.3.2/ph_baseliner/codes/
+-rw-r--r--   0 runner     (501) staff       (20)    13031 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/codes/ECCCNYS_2020.json
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/codes/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2072 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/codes/lighting_space_types.py
+-rw-r--r--   0 runner     (501) staff       (20)    17467 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/codes/model.py
+-rw-r--r--   0 runner     (501) staff       (20)     1406 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/codes/options.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:53.345877 PH-Baseliner-1.3.2/ph_baseliner/phpp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phpp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4691 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phpp/areas.py
+-rw-r--r--   0 runner     (501) staff       (20)     1484 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phpp/components.py
+-rw-r--r--   0 runner     (501) staff       (20)     2510 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phpp/lighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     3285 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phpp/u_values.py
+-rw-r--r--   0 runner     (501) staff       (20)     5618 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phpp/windows.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:53.347136 PH-Baseliner-1.3.2/ph_baseliner/phx/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phx/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2526 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phx/areas.py
+-rw-r--r--   0 runner     (501) staff       (20)     2583 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phx/constructions.py
+-rw-r--r--   0 runner     (501) staff       (20)      488 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phx/lighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     7637 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/ph_baseliner/phx/windows.py
+-rw-r--r--   0 runner     (501) staff       (20)       96 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)      800 2024-04-05 22:52:53.348547 PH-Baseliner-1.3.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2024-04-05 22:51:45.000000 PH-Baseliner-1.3.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PH-Baseliner-1.3.1/.github/workflows/ci.yaml` & `PH-Baseliner-1.3.2/.github/workflows/ci.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 jobs:
   test:
     name: Unit tests
 
     runs-on: macos-latest
     strategy:
       matrix:
-        python-version: [3.7]
+        python-version: [3.10.14]
     
     steps:
       - uses: actions/checkout@v2
       - name: set up Python
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
@@ -35,15 +35,15 @@
     needs: test
     if: github.ref == 'refs/heads/main' && github.repository_owner == 'ph-tools'
     steps:
       - uses: actions/checkout@v2
       - name: set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: 3.7
+          python-version: 3.10.14
       
       - name: set up node  # we need node for for semantic release
         uses: actions/setup-node@v2.1.2
         with:
           node-version: 14.2.0
       
       - name: install python dependencies
```

### Comparing `PH-Baseliner-1.3.1/LICENSE` & `PH-Baseliner-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/PH_Baseliner.egg-info/PKG-INFO` & `PH-Baseliner-1.3.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,35 @@
-Metadata-Version: 2.1
-Name: PH-Baseliner
-Version: 1.3.1
-Summary: Tools to automatically setup the code-minimum Baseline values for Passive House models.
-Home-page: https://github.com/PH-Tools/PH_Baseliner
-Author: PH-Tools
-Author-email: phtools@bldgtyp.com
-License: GPLv3+
-Description: # PH-Baseliner:
-        Tools to automatically setup the code-minimum 'Baseline' values for Passive House models.
-        
-        ## Usage:
-        The most basic usage is a to edit the values of an existing PHPP file to match 
-        a desired code-minimum configuration.
-        ```python
-        >>> # --- Connect to an instance of Excel with your PHPP file open.
-        >>> import xlwings as xw
-        >>> from PHX.xl import xl_app
-        >>> from PHX.PHPP import phpp_app
-        >>> xl = xl_app.XLConnection(xl_framework=xw)
-        >>> _phpp_conn = phpp_app.PHPPConnection(xl)
-        >>> 
-        >>> # --- Load the Code baseline model you would like to follow.
-        >>> import pathlib
-        >>> from ph_baseliner.codes.model import BaselineCode
-        >>> baseline_code_file_path = pathlib.Path(".", "ph_baseliner", "codes", "2020_ECCCNY.json")
-        >>> _baseline_code = BaselineCode.parse_file(baseline_code_file_path)
-        >>> 
-        >>> # --- Set the PHPP values as desired in the various Worksheets
-        >>> from ph_baseliner.codes.options import ClimateZones
-        >>> from ph_baseliner.phpp.areas import set_baseline_envelope_constructions
-        >>> set_baseline_envelope_constructions(_phpp_conn, _baseline_code, ClimateZones.CZ4)
-        ```
-        
-        - - -
-        Note: The baseliner will change the values of the PHPP file, and so you should 
-        be sure to make a backup copy before using this tool.
-        
-        - - - 
-        ![Tests](https://github.com/PH-Tools/PHX/actions/workflows/ci.yaml/badge.svg )
-        ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
-        [![IronPython](https://img.shields.io/badge/ironpython-2.7-red.svg)](https://github.com/IronLanguages/ironpython2/releases/tag/ipy-2.7.8/)
-        ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
+# PH-Baseliner:
+Tools to automatically setup the code-minimum 'Baseline' values for Passive House models.
+
+## Usage:
+The most basic usage is a to edit the values of an existing PHPP file to match 
+a desired code-minimum configuration.
+```python
+>>> # --- Connect to an instance of Excel with your PHPP file open.
+>>> import xlwings as xw
+>>> from PHX.xl import xl_app
+>>> from PHX.PHPP import phpp_app
+>>> xl = xl_app.XLConnection(xl_framework=xw)
+>>> _phpp_conn = phpp_app.PHPPConnection(xl)
+>>> 
+>>> # --- Load the Code baseline model you would like to follow.
+>>> import pathlib
+>>> from ph_baseliner.codes.model import BaselineCode
+>>> baseline_code_file_path = pathlib.Path(".", "ph_baseliner", "codes", "2020_ECCCNY.json")
+>>> _baseline_code = BaselineCode.parse_file(baseline_code_file_path)
+>>> 
+>>> # --- Set the PHPP values as desired in the various Worksheets
+>>> from ph_baseliner.codes.options import ClimateZones
+>>> from ph_baseliner.phpp.areas import set_baseline_envelope_constructions
+>>> set_baseline_envelope_constructions(_phpp_conn, _baseline_code, ClimateZones.CZ4)
+```
+
+- - -
+Note: The baseliner will change the values of the PHPP file, and so you should 
+be sure to make a backup copy before using this tool.
+
+- - - 
+![Tests](https://github.com/PH-Tools/PHX/actions/workflows/ci.yaml/badge.svg )
+![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
+[![IronPython](https://img.shields.io/badge/ironpython-2.7-red.svg)](https://github.com/IronLanguages/ironpython2/releases/tag/ipy-2.7.8/)
+![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
```

### Comparing `PH-Baseliner-1.3.1/PH_Baseliner.egg-info/SOURCES.txt` & `PH-Baseliner-1.3.2/PH_Baseliner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/codes/ECCCNYS_2020.json` & `PH-Baseliner-1.3.2/ph_baseliner/codes/ECCCNYS_2020.json`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/codes/lighting_space_types.py` & `PH-Baseliner-1.3.2/ph_baseliner/codes/lighting_space_types.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/codes/model.py` & `PH-Baseliner-1.3.2/ph_baseliner/codes/model.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/codes/options.py` & `PH-Baseliner-1.3.2/ph_baseliner/codes/options.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/phpp/areas.py` & `PH-Baseliner-1.3.2/ph_baseliner/phpp/areas.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/phpp/components.py` & `PH-Baseliner-1.3.2/ph_baseliner/phpp/components.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/phpp/lighting.py` & `PH-Baseliner-1.3.2/ph_baseliner/phpp/lighting.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/phpp/u_values.py` & `PH-Baseliner-1.3.2/ph_baseliner/phpp/u_values.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/phpp/windows.py` & `PH-Baseliner-1.3.2/ph_baseliner/phpp/windows.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/phx/areas.py` & `PH-Baseliner-1.3.2/ph_baseliner/phx/areas.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/phx/constructions.py` & `PH-Baseliner-1.3.2/ph_baseliner/phx/constructions.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/ph_baseliner/phx/windows.py` & `PH-Baseliner-1.3.2/ph_baseliner/phx/windows.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.3.1/setup.cfg` & `PH-Baseliner-1.3.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 url = https://github.com/PH-Tools/PH_Baseliner
 license = GPLv3+
 license_files = LICENSE
 name = PH-Baseliner
 description = Tools to automatically setup the code-minimum Baseline values for Passive House models.
 classifiers = 
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 	Typing :: Typed
 
 [options]
 include_package_data = True
```

