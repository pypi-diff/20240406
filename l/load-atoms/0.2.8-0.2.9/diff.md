# Comparing `tmp/load-atoms-0.2.8.tar.gz` & `tmp/load-atoms-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "load-atoms-0.2.8.tar", last modified: Fri Feb 23 15:08:52 2024, max compression
+gzip compressed data, was "load-atoms-0.2.9.tar", last modified: Mon Feb 26 12:39:53 2024, max compression
```

## Comparing `load-atoms-0.2.8.tar` & `load-atoms-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:08:52.961214 load-atoms-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-23 15:08:10.000000 load-atoms-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-23 15:08:10.000000 load-atoms-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-02-23 15:08:52.961214 load-atoms-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-02-23 15:08:10.000000 load-atoms-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-02-23 15:08:10.000000 load-atoms-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 15:08:52.961214 load-atoms-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:08:52.949215 load-atoms-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:08:52.953215 load-atoms-0.2.8/src/load_atoms/
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16811 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/atoms_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:08:52.953215 load-atoms-0.2.8/src/load_atoms/database/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/database/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/database/database_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/database/internet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:08:52.957214 load-atoms-0.2.8/src/load_atoms/database/processing/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/database/processing/1-dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/database/processing/AC-2D-22.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/database/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19136 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/database/processing/bad_qm9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/database/processing/read_qm9_xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:08:52.957214 load-atoms-0.2.8/src/load_atoms/visualisation/
--rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/visualisation/view.js
--rw-r--r--   0 runner    (1001) docker     (127)   853705 2024-02-23 15:08:10.000000 load-atoms-0.2.8/src/load_atoms/visualisation/x3d.script
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:08:52.957214 load-atoms-0.2.8/src/load_atoms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-02-23 15:08:52.000000 load-atoms-0.2.8/src/load_atoms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-23 15:08:52.000000 load-atoms-0.2.8/src/load_atoms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 15:08:52.000000 load-atoms-0.2.8/src/load_atoms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-23 15:08:52.000000 load-atoms-0.2.8/src/load_atoms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-23 15:08:52.000000 load-atoms-0.2.8/src/load_atoms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:08:52.957214 load-atoms-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-02-23 15:08:10.000000 load-atoms-0.2.8/tests/test_atoms_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-02-23 15:08:10.000000 load-atoms-0.2.8/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-23 15:08:10.000000 load-atoms-0.2.8/tests/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:39:53.303996 load-atoms-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-26 12:39:04.000000 load-atoms-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-26 12:39:04.000000 load-atoms-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-02-26 12:39:53.303996 load-atoms-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-02-26 12:39:04.000000 load-atoms-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-02-26 12:39:05.000000 load-atoms-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 12:39:53.303996 load-atoms-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:39:53.295996 load-atoms-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:39:53.295996 load-atoms-0.2.9/src/load_atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16811 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/atoms_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:39:53.299996 load-atoms-0.2.9/src/load_atoms/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/database/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/database/database_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/database/internet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:39:53.299996 load-atoms-0.2.9/src/load_atoms/database/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/database/processing/1-dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/database/processing/AC-2D-22.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/database/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19136 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/database/processing/bad_qm9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/database/processing/read_qm9_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:39:53.299996 load-atoms-0.2.9/src/load_atoms/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/visualisation/view.js
+-rw-r--r--   0 runner    (1001) docker     (127)   853705 2024-02-26 12:39:05.000000 load-atoms-0.2.9/src/load_atoms/visualisation/x3d.script
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:39:53.299996 load-atoms-0.2.9/src/load_atoms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-02-26 12:39:53.000000 load-atoms-0.2.9/src/load_atoms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-26 12:39:53.000000 load-atoms-0.2.9/src/load_atoms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 12:39:53.000000 load-atoms-0.2.9/src/load_atoms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-26 12:39:53.000000 load-atoms-0.2.9/src/load_atoms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-26 12:39:53.000000 load-atoms-0.2.9/src/load_atoms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:39:53.299996 load-atoms-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-02-26 12:39:05.000000 load-atoms-0.2.9/tests/test_atoms_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-02-26 12:39:05.000000 load-atoms-0.2.9/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-26 12:39:05.000000 load-atoms-0.2.9/tests/test_view.py
```

### Comparing `load-atoms-0.2.8/LICENSE` & `load-atoms-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/PKG-INFO` & `load-atoms-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: load-atoms
-Version: 0.2.8
+Version: 0.2.9
 Summary: Large Open Access Datasets for Atomistic Materials Science (LOAD-AtoMS)
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,14 +52,15 @@
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx_autodoc_typehints; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: sphinx_copybutton; extra == "dev"
 Requires-Dist: sphinx-codeautolink; extra == "dev"
+Requires-Dist: sphinxext-opengraph; extra == "dev"
 
 > [!WARNING]
 > This project is under active development. Until version 1.0.0 is released, breaking changes to the API may occur with no notice.
 > 
 <div align="center">
     <a href="https://jla-gardner.github.io/load-atoms/">
         <img src="https://raw.githubusercontent.com/jla-gardner/load-atoms/main/docs/source/logo.svg" width="50%"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: load-atoms Version: 0.2.8 Summary: Large Open
+Metadata-Version: 2.1 Name: load-atoms Version: 0.2.9 Summary: Large Open
 Access Datasets for Atomistic Materials Science (LOAD-AtoMS) Author-email: John
 Gardner
 gmail.com> License: MIT License Copyright (c) 2023 John Gardner Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -26,17 +26,18 @@
 pytest==7.2.0; extra == "dev" Requires-Dist: sphinx; extra == "dev" Requires-
 Dist: furo; extra == "dev" Requires-Dist: nbsphinx; extra == "dev" Requires-
 Dist: sphinx-autobuild; extra == "dev" Requires-Dist: pytest-cov; extra ==
 "dev" Requires-Dist: build; extra == "dev" Requires-Dist: bumpver; extra ==
 "dev" Requires-Dist: twine; extra == "dev" Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx_autodoc_typehints; extra == "dev" Requires-Dist: sphinx-
 design; extra == "dev" Requires-Dist: sphinx_copybutton; extra == "dev"
-Requires-Dist: sphinx-codeautolink; extra == "dev" > [!WARNING] > This project
-is under active development. Until version 1.0.0 is released, breaking changes
-to the API may occur with no notice. >
+Requires-Dist: sphinx-codeautolink; extra == "dev" Requires-Dist: sphinxext-
+opengraph; extra == "dev" > [!WARNING] > This project is under active
+development. Until version 1.0.0 is released, breaking changes to the API may
+occur with no notice. >
   _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_j_l_a_-_g_a_r_d_n_e_r_/_l_o_a_d_-_a_t_o_m_s_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/
                                    _l_o_g_o_._s_v_g_]
  [![PyPI](https://img.shields.io/pypi/v/load-atoms)](https://pypi.org/project/
     load-atoms/) [![GitHub](https://img.shields.io/badge/license-MIT-blue)]
   (LICENSE) [![](https://github.com/jla-gardner/load-atoms/actions/workflows/
  tests.yaml/badge.svg?branch=main)](https://github.com/jla-gardner/load-atoms/
  actions/workflows/tests.yaml) [![codecov](https://codecov.io/gh/jla-gardner/
```

### Comparing `load-atoms-0.2.8/README.md` & `load-atoms-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/pyproject.toml` & `load-atoms-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "load-atoms"
-version = "0.2.8"
+version = "0.2.9"
 description = "Large Open Access Datasets for Atomistic Materials Science (LOAD-AtoMS)"
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -40,21 +40,22 @@
     "bumpver",
     "twine",
     "ruff",
     "sphinx_autodoc_typehints",
     "sphinx-design",
     "sphinx_copybutton",
     "sphinx-codeautolink",
+    "sphinxext-opengraph",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/load-atoms"
 
 [tool.bumpver]
-current_version = "0.2.8"
+current_version = "0.2.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
@@ -71,15 +72,15 @@
 indent-width = 4
 target-version = "py38"
 
 [tool.ruff.lint]
 select = ["E", "F", "UP", "B", "SIM", "I"]
 fixable = ["ALL"]
 unfixable = []
-ignore = ["SIM300", "E402", "E703", "B017"]
+ignore = ["SIM300", "E402", "E703", "B017", "I001"]
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
 skip-magic-trailing-comma = false
 line-ending = "auto"
```

### Comparing `load-atoms-0.2.8/src/load_atoms/__init__.py` & `load-atoms-0.2.9/src/load_atoms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import ase
 from ase.io import read
 
 from .atoms_dataset import AtomsDataset, DescribedDataset
 from .visualisation import view
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 __all__ = ["load_dataset", "view"]
 
 
 def load_dataset(
     thing: str | list[ase.Atoms] | Path,
     root: str | Path | None = None,
 ) -> AtomsDataset:
```

### Comparing `load-atoms-0.2.8/src/load_atoms/atoms_dataset.py` & `load-atoms-0.2.9/src/load_atoms/atoms_dataset.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/database/backend.py` & `load-atoms-0.2.9/src/load_atoms/database/backend.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/database/database_entry.py` & `load-atoms-0.2.9/src/load_atoms/database/database_entry.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/database/internet.py` & `load-atoms-0.2.9/src/load_atoms/database/internet.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/database/processing/AC-2D-22.py` & `load-atoms-0.2.9/src/load_atoms/database/processing/AC-2D-22.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/database/processing/__init__.py` & `load-atoms-0.2.9/src/load_atoms/database/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/database/processing/bad_qm9.txt` & `load-atoms-0.2.9/src/load_atoms/database/processing/bad_qm9.txt`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/database/processing/read_qm9_xyz.py` & `load-atoms-0.2.9/src/load_atoms/database/processing/read_qm9_xyz.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/progress.py` & `load-atoms-0.2.9/src/load_atoms/progress.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/utils.py` & `load-atoms-0.2.9/src/load_atoms/utils.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/visualisation/__init__.py` & `load-atoms-0.2.9/src/load_atoms/visualisation/__init__.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/visualisation/view.js` & `load-atoms-0.2.9/src/load_atoms/visualisation/view.js`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms/visualisation/x3d.script` & `load-atoms-0.2.9/src/load_atoms/visualisation/x3d.script`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/src/load_atoms.egg-info/PKG-INFO` & `load-atoms-0.2.9/src/load_atoms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: load-atoms
-Version: 0.2.8
+Version: 0.2.9
 Summary: Large Open Access Datasets for Atomistic Materials Science (LOAD-AtoMS)
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,14 +52,15 @@
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx_autodoc_typehints; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: sphinx_copybutton; extra == "dev"
 Requires-Dist: sphinx-codeautolink; extra == "dev"
+Requires-Dist: sphinxext-opengraph; extra == "dev"
 
 > [!WARNING]
 > This project is under active development. Until version 1.0.0 is released, breaking changes to the API may occur with no notice.
 > 
 <div align="center">
     <a href="https://jla-gardner.github.io/load-atoms/">
         <img src="https://raw.githubusercontent.com/jla-gardner/load-atoms/main/docs/source/logo.svg" width="50%"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: load-atoms Version: 0.2.8 Summary: Large Open
+Metadata-Version: 2.1 Name: load-atoms Version: 0.2.9 Summary: Large Open
 Access Datasets for Atomistic Materials Science (LOAD-AtoMS) Author-email: John
 Gardner
 gmail.com> License: MIT License Copyright (c) 2023 John Gardner Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -26,17 +26,18 @@
 pytest==7.2.0; extra == "dev" Requires-Dist: sphinx; extra == "dev" Requires-
 Dist: furo; extra == "dev" Requires-Dist: nbsphinx; extra == "dev" Requires-
 Dist: sphinx-autobuild; extra == "dev" Requires-Dist: pytest-cov; extra ==
 "dev" Requires-Dist: build; extra == "dev" Requires-Dist: bumpver; extra ==
 "dev" Requires-Dist: twine; extra == "dev" Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx_autodoc_typehints; extra == "dev" Requires-Dist: sphinx-
 design; extra == "dev" Requires-Dist: sphinx_copybutton; extra == "dev"
-Requires-Dist: sphinx-codeautolink; extra == "dev" > [!WARNING] > This project
-is under active development. Until version 1.0.0 is released, breaking changes
-to the API may occur with no notice. >
+Requires-Dist: sphinx-codeautolink; extra == "dev" Requires-Dist: sphinxext-
+opengraph; extra == "dev" > [!WARNING] > This project is under active
+development. Until version 1.0.0 is released, breaking changes to the API may
+occur with no notice. >
   _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_j_l_a_-_g_a_r_d_n_e_r_/_l_o_a_d_-_a_t_o_m_s_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/
                                    _l_o_g_o_._s_v_g_]
  [![PyPI](https://img.shields.io/pypi/v/load-atoms)](https://pypi.org/project/
     load-atoms/) [![GitHub](https://img.shields.io/badge/license-MIT-blue)]
   (LICENSE) [![](https://github.com/jla-gardner/load-atoms/actions/workflows/
  tests.yaml/badge.svg?branch=main)](https://github.com/jla-gardner/load-atoms/
  actions/workflows/tests.yaml) [![codecov](https://codecov.io/gh/jla-gardner/
```

### Comparing `load-atoms-0.2.8/src/load_atoms.egg-info/SOURCES.txt` & `load-atoms-0.2.9/src/load_atoms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/tests/test_atoms_dataset.py` & `load-atoms-0.2.9/tests/test_atoms_dataset.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/tests/test_util.py` & `load-atoms-0.2.9/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.2.8/tests/test_view.py` & `load-atoms-0.2.9/tests/test_view.py`

 * *Files identical despite different names*

