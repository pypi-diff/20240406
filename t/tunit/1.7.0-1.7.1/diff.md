# Comparing `tmp/tunit-1.7.0.tar.gz` & `tmp/tunit-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tunit-1.7.0.tar", last modified: Wed Apr  3 17:28:49 2024, max compression
+gzip compressed data, was "dist/tunit-1.7.1.tar", last modified: Sat Apr  6 13:32:41 2024, max compression
```

## Comparing `tunit-1.7.0.tar` & `tunit-1.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2022-04-24 18:13:16.000000 tunit-1.7.0/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)      127 2024-04-02 15:00:40.000000 tunit-1.7.0/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4788 2024-04-03 17:28:49.000000 tunit-1.7.0/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4258 2024-04-03 17:24:14.000000 tunit-1.7.0/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      167 2024-04-03 17:09:49.000000 tunit-1.7.0/pkg/tunit/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      920 2024-04-03 16:55:59.000000 tunit-1.7.0/pkg/tunit/config.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)    10100 2024-03-28 17:47:12.000000 tunit-1.7.0/pkg/tunit/core.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit/markup/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-02 15:19:52.000000 tunit-1.7.0/pkg/tunit/markup/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1734 2024-04-03 17:01:40.000000 tunit-1.7.0/pkg/tunit/markup/json.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2571 2024-04-03 17:02:12.000000 tunit-1.7.0/pkg/tunit/markup/yaml.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 tunit-1.7.0/pkg/tunit/py.typed
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1577 2024-03-28 17:38:44.000000 tunit-1.7.0/pkg/tunit/unit.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4788 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      495 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/not-zip-safe
--rw-r--r--   0 pawel     (1000) pawel     (1000)       83 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/requires.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        6 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/top_level.txt
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/requirements/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/requirements/extra/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       31 2024-03-28 22:08:02.000000 tunit-1.7.0/requirements/extra/json.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       42 2024-04-02 16:04:05.000000 tunit-1.7.0/requirements/extra/yaml.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-03 17:05:26.000000 tunit-1.7.0/requirements/release.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-03 17:28:49.000000 tunit-1.7.0/setup.cfg
--rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2827 2024-04-03 17:08:14.000000 tunit-1.7.0/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2022-04-24 18:13:16.000000 tunit-1.7.1/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      127 2024-04-02 15:00:40.000000 tunit-1.7.1/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4912 2024-04-06 13:32:41.000000 tunit-1.7.1/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4362 2024-04-06 13:30:05.000000 tunit-1.7.1/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      167 2024-04-06 13:30:29.000000 tunit-1.7.1/pkg/tunit/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      920 2024-04-03 16:55:59.000000 tunit-1.7.1/pkg/tunit/config.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)    10100 2024-03-28 17:47:12.000000 tunit-1.7.1/pkg/tunit/core.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit/markup/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-02 15:19:52.000000 tunit-1.7.1/pkg/tunit/markup/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1734 2024-04-03 17:01:40.000000 tunit-1.7.1/pkg/tunit/markup/json.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2571 2024-04-03 17:02:12.000000 tunit-1.7.1/pkg/tunit/markup/yaml.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 tunit-1.7.1/pkg/tunit/py.typed
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1577 2024-03-28 17:38:44.000000 tunit-1.7.1/pkg/tunit/unit.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4912 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      495 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/not-zip-safe
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      157 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/requires.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        6 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/top_level.txt
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/requirements/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/requirements/extra/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       31 2024-03-28 22:08:02.000000 tunit-1.7.1/requirements/extra/json.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       42 2024-04-02 16:04:05.000000 tunit-1.7.1/requirements/extra/yaml.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-03 17:05:26.000000 tunit-1.7.1/requirements/release.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-06 13:32:41.000000 tunit-1.7.1/setup.cfg
+-rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2974 2024-04-06 13:28:00.000000 tunit-1.7.1/setup.py
```

### Comparing `tunit-1.7.0/LICENSE.txt` & `tunit-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tunit-1.7.0/PKG-INFO` & `tunit-1.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: tunit
-Version: 1.7.0
+Version: 1.7.1
 Summary: Time unit types. For transparency safety and readability.
 Home-page: https://bitbucket.org/massultidev/tunit/
 Author: P.J. Grochowski
 Author-email: pawel.grochowski.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: json
 Provides-Extra: yaml
+Provides-Extra: all
 License-File: LICENSE.txt
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI license](https://img.shields.io/pypi/l/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![Downloads](https://static.pepy.tech/badge/tunit)](https://pepy.tech/project/tunit)
 
 # TUnit
 ---
 Time unit types. For transparency, safety and readability.
 
 ## Installation:
 
 ```bash
-pip install tunit # Base package
-pip install tunit[json] # JSON serialization/deserialization support
-pip install tunit[yaml] # YAML serialization/deserialization support
+pip install tunit # Install just the base package
+pip install tunit[json] # Install with extra JSON serialization/deserialization support
+pip install tunit[yaml] # Install with extra YAML serialization/deserialization support
+pip install tunit[all] # Install with all extras
 ```
 
 ## Examples:
 
 Type conversions:
 ```python
 from tunit.unit import Days, Hours, Minutes, Seconds, Milliseconds
```

### Comparing `tunit-1.7.0/README.md` & `tunit-1.7.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 # TUnit
 ---
 Time unit types. For transparency, safety and readability.
 
 ## Installation:
 
 ```bash
-pip install tunit # Base package
-pip install tunit[json] # JSON serialization/deserialization support
-pip install tunit[yaml] # YAML serialization/deserialization support
+pip install tunit # Install just the base package
+pip install tunit[json] # Install with extra JSON serialization/deserialization support
+pip install tunit[yaml] # Install with extra YAML serialization/deserialization support
+pip install tunit[all] # Install with all extras
 ```
 
 ## Examples:
 
 Type conversions:
 ```python
 from tunit.unit import Days, Hours, Minutes, Seconds, Milliseconds
```

### Comparing `tunit-1.7.0/pkg/tunit/config.py` & `tunit-1.7.1/pkg/tunit/config.py`

 * *Files identical despite different names*

### Comparing `tunit-1.7.0/pkg/tunit/core.py` & `tunit-1.7.1/pkg/tunit/core.py`

 * *Files identical despite different names*

### Comparing `tunit-1.7.0/pkg/tunit/markup/json.py` & `tunit-1.7.1/pkg/tunit/markup/json.py`

 * *Files identical despite different names*

### Comparing `tunit-1.7.0/pkg/tunit/markup/yaml.py` & `tunit-1.7.1/pkg/tunit/markup/yaml.py`

 * *Files identical despite different names*

### Comparing `tunit-1.7.0/pkg/tunit/unit.py` & `tunit-1.7.1/pkg/tunit/unit.py`

 * *Files identical despite different names*

### Comparing `tunit-1.7.0/pkg/tunit.egg-info/PKG-INFO` & `tunit-1.7.1/pkg/tunit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: tunit
-Version: 1.7.0
+Version: 1.7.1
 Summary: Time unit types. For transparency safety and readability.
 Home-page: https://bitbucket.org/massultidev/tunit/
 Author: P.J. Grochowski
 Author-email: pawel.grochowski.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: json
 Provides-Extra: yaml
+Provides-Extra: all
 License-File: LICENSE.txt
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI license](https://img.shields.io/pypi/l/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![Downloads](https://static.pepy.tech/badge/tunit)](https://pepy.tech/project/tunit)
 
 # TUnit
 ---
 Time unit types. For transparency, safety and readability.
 
 ## Installation:
 
 ```bash
-pip install tunit # Base package
-pip install tunit[json] # JSON serialization/deserialization support
-pip install tunit[yaml] # YAML serialization/deserialization support
+pip install tunit # Install just the base package
+pip install tunit[json] # Install with extra JSON serialization/deserialization support
+pip install tunit[yaml] # Install with extra YAML serialization/deserialization support
+pip install tunit[all] # Install with all extras
 ```
 
 ## Examples:
 
 Type conversions:
 ```python
 from tunit.unit import Days, Hours, Minutes, Seconds, Milliseconds
```

### Comparing `tunit-1.7.0/setup.py` & `tunit-1.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
+import itertools
 import shutil
 import sys
 from pathlib import Path
 from typing import List, Tuple
 
 from setuptools import Command, find_packages, setup
 
@@ -61,14 +62,20 @@
             print(f"Removing: {path}")
             shutil.rmtree(path)
 
 
 def main():
     assert_working_dir()
 
+    extra_requirements = dict([
+        get_extra_requirements('json'),
+        get_extra_requirements('yaml'),
+    ])
+    extra_requirements['all'] = list(itertools.chain.from_iterable(extra_requirements.values()))
+
     setup(
         name=__package__,
         version=__version__,
         license='MIT',
         url='https://bitbucket.org/massultidev/tunit/',
         author='P.J. Grochowski',
         author_email='pawel.grochowski.dev@gmail.com',
@@ -76,18 +83,15 @@
         long_description=read_file(DIR_ROOT / 'README.md'),
         long_description_content_type='text/markdown',
         package_dir={'': NAME_PACKAGE_ROOT},
         packages=find_packages(NAME_PACKAGE_ROOT),
         include_package_data=True,
         zip_safe=False,
         install_requires=get_requirements(),
-        extras_require=dict([
-            get_extra_requirements('json'),
-            get_extra_requirements('yaml'),
-        ]),
+        extras_require=extra_requirements,
         python_requires='>=3.7',
         classifiers=[
             "Programming Language :: Python :: 3.7",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
         ],
         cmdclass={
```

