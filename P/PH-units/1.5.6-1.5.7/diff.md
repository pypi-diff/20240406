# Comparing `tmp/PH-units-1.5.6.tar.gz` & `tmp/PH-units-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-units-1.5.6.tar", last modified: Tue Dec 19 14:30:24 2023, max compression
+gzip compressed data, was "PH-units-1.5.7.tar", last modified: Fri Apr  5 22:52:40 2024, max compression
```

## Comparing `PH-units-1.5.6.tar` & `PH-units-1.5.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-12-19 14:30:24.000000 PH-units-1.5.6/
--rw-r--r--   0 runner     (501) staff       (20)       66 2023-12-19 14:29:14.000000 PH-units-1.5.6/.gitattributes
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-12-19 14:30:24.000000 PH-units-1.5.6/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-12-19 14:30:24.000000 PH-units-1.5.6/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1781 2023-12-19 14:29:14.000000 PH-units-1.5.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35129 2023-12-19 14:29:14.000000 PH-units-1.5.6/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-12-19 14:30:24.000000 PH-units-1.5.6/PH_units.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     4022 2023-12-19 14:30:23.000000 PH-units-1.5.6/PH_units.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      781 2023-12-19 14:30:24.000000 PH-units-1.5.6/PH_units.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-12-19 14:30:23.000000 PH-units-1.5.6/PH_units.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2023-12-19 14:30:23.000000 PH-units-1.5.6/PH_units.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     4022 2023-12-19 14:30:24.000000 PH-units-1.5.6/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2711 2023-12-19 14:29:14.000000 PH-units-1.5.6/README.md
--rw-r--r--   0 runner     (501) staff       (20)       50 2023-12-19 14:29:14.000000 PH-units-1.5.6/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-12-19 14:30:24.000000 PH-units-1.5.6/ph_units/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6294 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/converter.py
--rw-r--r--   0 runner     (501) staff       (20)     2036 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/parser.py
--rw-r--r--   0 runner     (501) staff       (20)     8602 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_type.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-12-19 14:30:24.000000 PH-units-1.5.6/ph_units/unit_types/
--rw-r--r--   0 runner     (501) staff       (20)     2999 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      371 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/_base.py
--rw-r--r--   0 runner     (501) staff       (20)      855 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/area.py
--rw-r--r--   0 runner     (501) staff       (20)     1220 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/density.py
--rw-r--r--   0 runner     (501) staff       (20)      763 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/emissions_factors.py
--rw-r--r--   0 runner     (501) staff       (20)     7362 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/energy.py
--rw-r--r--   0 runner     (501) staff       (20)     2681 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/envelope.py
--rw-r--r--   0 runner     (501) staff       (20)     1459 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/length.py
--rw-r--r--   0 runner     (501) staff       (20)      584 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/moisture_vapor_resistance.py
--rw-r--r--   0 runner     (501) staff       (20)     2489 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/power.py
--rw-r--r--   0 runner     (501) staff       (20)     1408 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/speed.py
--rw-r--r--   0 runner     (501) staff       (20)     1030 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/temperature.py
--rw-r--r--   0 runner     (501) staff       (20)     1196 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/volume.py
--rw-r--r--   0 runner     (501) staff       (20)     2354 2023-12-19 14:29:14.000000 PH-units-1.5.6/ph_units/unit_types/volume_flow.py
--rw-r--r--   0 runner     (501) staff       (20)      219 2023-12-19 14:29:14.000000 PH-units-1.5.6/sandbox.py
--rw-r--r--   0 runner     (501) staff       (20)      832 2023-12-19 14:30:24.000000 PH-units-1.5.6/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-12-19 14:29:14.000000 PH-units-1.5.6/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:40.259766 PH-units-1.5.7/
+-rw-r--r--   0 runner     (501) staff       (20)       66 2024-04-05 22:51:31.000000 PH-units-1.5.7/.gitattributes
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:40.245466 PH-units-1.5.7/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:40.250905 PH-units-1.5.7/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1789 2024-04-05 22:51:31.000000 PH-units-1.5.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35129 2024-04-05 22:51:31.000000 PH-units-1.5.7/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:40.252541 PH-units-1.5.7/PH_units.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3436 2024-04-05 22:52:40.000000 PH-units-1.5.7/PH_units.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      781 2024-04-05 22:52:40.000000 PH-units-1.5.7/PH_units.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-05 22:52:40.000000 PH-units-1.5.7/PH_units.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-05 22:52:40.000000 PH-units-1.5.7/PH_units.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     3436 2024-04-05 22:52:40.260100 PH-units-1.5.7/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2711 2024-04-05 22:51:31.000000 PH-units-1.5.7/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       50 2024-04-05 22:51:31.000000 PH-units-1.5.7/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:40.254119 PH-units-1.5.7/ph_units/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6294 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/converter.py
+-rw-r--r--   0 runner     (501) staff       (20)     2036 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/parser.py
+-rw-r--r--   0 runner     (501) staff       (20)     8602 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_type.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-05 22:52:40.259486 PH-units-1.5.7/ph_units/unit_types/
+-rw-r--r--   0 runner     (501) staff       (20)     2999 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      371 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/_base.py
+-rw-r--r--   0 runner     (501) staff       (20)      855 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/area.py
+-rw-r--r--   0 runner     (501) staff       (20)     1220 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/density.py
+-rw-r--r--   0 runner     (501) staff       (20)      763 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/emissions_factors.py
+-rw-r--r--   0 runner     (501) staff       (20)     7362 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/energy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2681 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/envelope.py
+-rw-r--r--   0 runner     (501) staff       (20)     1459 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/length.py
+-rw-r--r--   0 runner     (501) staff       (20)      584 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/moisture_vapor_resistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     2489 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/power.py
+-rw-r--r--   0 runner     (501) staff       (20)     1408 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/speed.py
+-rw-r--r--   0 runner     (501) staff       (20)     1030 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/temperature.py
+-rw-r--r--   0 runner     (501) staff       (20)     1196 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/volume.py
+-rw-r--r--   0 runner     (501) staff       (20)     2354 2024-04-05 22:51:31.000000 PH-units-1.5.7/ph_units/unit_types/volume_flow.py
+-rw-r--r--   0 runner     (501) staff       (20)      219 2024-04-05 22:51:31.000000 PH-units-1.5.7/sandbox.py
+-rw-r--r--   0 runner     (501) staff       (20)      831 2024-04-05 22:52:40.261311 PH-units-1.5.7/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2024-04-05 22:51:31.000000 PH-units-1.5.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PH-units-1.5.6/.github/workflows/ci.yaml` & `PH-units-1.5.7/.github/workflows/ci.yaml`

 * *Files 2% similar despite different names*

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
@@ -32,15 +32,15 @@
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

### Comparing `PH-units-1.5.6/LICENSE` & `PH-units-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/PH_units.egg-info/SOURCES.txt` & `PH-units-1.5.7/PH_units.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/README.md` & `PH-units-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/converter.py` & `PH-units-1.5.7/ph_units/converter.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/parser.py` & `PH-units-1.5.7/ph_units/parser.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_type.py` & `PH-units-1.5.7/ph_units/unit_type.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/__init__.py` & `PH-units-1.5.7/ph_units/unit_types/__init__.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/area.py` & `PH-units-1.5.7/ph_units/unit_types/area.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/density.py` & `PH-units-1.5.7/ph_units/unit_types/density.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/emissions_factors.py` & `PH-units-1.5.7/ph_units/unit_types/emissions_factors.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/energy.py` & `PH-units-1.5.7/ph_units/unit_types/energy.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/envelope.py` & `PH-units-1.5.7/ph_units/unit_types/envelope.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/length.py` & `PH-units-1.5.7/ph_units/unit_types/length.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/moisture_vapor_resistance.py` & `PH-units-1.5.7/ph_units/unit_types/moisture_vapor_resistance.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/power.py` & `PH-units-1.5.7/ph_units/unit_types/power.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/speed.py` & `PH-units-1.5.7/ph_units/unit_types/speed.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/temperature.py` & `PH-units-1.5.7/ph_units/unit_types/temperature.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/volume.py` & `PH-units-1.5.7/ph_units/unit_types/volume.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/ph_units/unit_types/volume_flow.py` & `PH-units-1.5.7/ph_units/unit_types/volume_flow.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.5.6/setup.cfg` & `PH-units-1.5.7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 author_email = phtools@bldgtyp.com
 url = https://github.com/PH-Tools/PH_units
 license = GPLv3+
 license_files = LICENSE
 name = PH-units
 description = Tools for working with common Passive House unit types
 classifiers = 
+	Programming Language :: Python :: 2
 	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 	Typing :: Typed
 
 [options]
 include_package_data = True
```

