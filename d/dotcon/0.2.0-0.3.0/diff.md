# Comparing `tmp/dotcon-0.2.0.tar.gz` & `tmp/dotcon-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotcon-0.2.0.tar", max compression
+gzip compressed data, was "dotcon-0.3.0.tar", max compression
```

## Comparing `dotcon-0.2.0.tar` & `dotcon-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      764 2024-04-06 10:31:09.119850 dotcon-0.2.0/dotcon/__init__.py
--rw-r--r--   0        0        0     1072 2024-04-05 13:39:29.045903 dotcon-0.2.0/LICENSE
--rw-r--r--   0        0        0     1265 2024-04-06 10:36:23.832292 dotcon-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      603 2024-04-06 10:38:00.395118 dotcon-0.2.0/README.md
--rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 dotcon-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      764 2024-04-06 10:41:53.245882 dotcon-0.3.0/dotcon/__init__.py
+-rw-r--r--   0        0        0     1072 2024-04-05 13:39:29.045903 dotcon-0.3.0/LICENSE
+-rw-r--r--   0        0        0      718 2024-04-06 13:25:23.675781 dotcon-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      617 2024-04-06 13:25:23.674781 dotcon-0.3.0/README.md
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 dotcon-0.3.0/PKG-INFO
```

### Comparing `dotcon-0.2.0/dotcon/__init__.py` & `dotcon-0.3.0/dotcon/__init__.py`

 * *Files identical despite different names*

### Comparing `dotcon-0.2.0/LICENSE` & `dotcon-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dotcon-0.2.0/pyproject.toml` & `dotcon-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,26 @@
-# [project]
-# name = "dot_dict"
-# requires-python = ">= 3.11"
-
-# authors = [{ name = "Aidan Inceer", email = "aidaninceer0@gmail.com" }]
-
-# description = "A simple package which converts a standard python dictionary to a dot accessible object."
-# readme = "README.md"
-# license = { file = "LICENSE" }
-
-# keywords = ["dot", "dict"]
-
-# classifiers = [
-#     "Development Status :: 3 - Alpha",
-#     "Intended Audience :: Developers",
-# ]
-
-# [project.urls]
-# Repository = "https://github.com/AidanInceer/DotDict"
-
-
-[tool.commitizen]
-version = "0.2.0"
-version_files = ["README.md", "pyproject.toml:version", "setup.py"]
-name = "cz_conventional_commits"
-tag_format = "$major.$minor.$patch"
-version_scheme = "semver"
-version_provider = "poetry"
-update_changelog_on_bump = true
-changelog_incremental = true
-
 [tool.poetry]
 name = "dotcon"
-version = "0.2.0"
+version = "0.3.0"
 description = "A simple package which converts a standard python dictionary to a dot accessible object."
 authors = ["AidanInceer <aidaninceer0@gmail.com>"]
 license = "LICENCE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pre-commit = "^3.7.0"
 pytest = "^8.1.1"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.commitizen]
+version = "0.3.0"
+version_files = ["README.md", "pyproject.toml:version"]
+name = "cz_conventional_commits"
+tag_format = "$major.$minor.$patch"
+version_scheme = "semver"
+version_provider = "poetry"
+update_changelog_on_bump = true
+changelog_incremental = true
```

### Comparing `dotcon-0.2.0/README.md` & `dotcon-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # DotConfig
 
 <a href="https://github.com/AidanInceer/DotDict">
-    <img alt="Static Badge" src="https://img.shields.io/badge/version-0.2.0-blue">
+    <img alt="Static Badge" src="https://img.shields.io/badge/version-0.3.0-blue">
 </a>
 
-A simple package which converts a standard python dictionary to a dot accessible object.
+A simple package which converts a standard python dictionary to a dot accessible configuration object.
 
 ## Installation
 
 ``` bash
 pip install dotcon
 ```
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 # DotConfig _[_S_t_a_t_i_c_ _B_a_d_g_e_]A simple package which converts a standard python
-dictionary to a dot accessible object. ## Installation ``` bash pip install
-dotcon ``` ## Usage ``` python from dotcon import DotConfig mydict = { "A": [1,
-2, 3, 4], "B": {"C": 5}, "D": "E", "F": None, } ddict = DotConfig(mydict)
-ddict.A >>> [1, 2, 3, 4] ddict.B >>> {"C": 5} ddict.B.C >>> 5 ddict.D >>> "E"
-ddict.F >>> None ```
+dictionary to a dot accessible configuration object. ## Installation ``` bash
+pip install dotcon ``` ## Usage ``` python from dotcon import DotConfig mydict
+= { "A": [1, 2, 3, 4], "B": {"C": 5}, "D": "E", "F": None, } ddict = DotConfig
+(mydict) ddict.A >>> [1, 2, 3, 4] ddict.B >>> {"C": 5} ddict.B.C >>> 5 ddict.D
+>>> "E" ddict.F >>> None ```
```

### Comparing `dotcon-0.2.0/PKG-INFO` & `dotcon-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotcon
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple package which converts a standard python dictionary to a dot accessible object.
 License: LICENCE
 Author: AidanInceer
 Author-email: aidaninceer0@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,18 +13,18 @@
 Requires-Dist: pre-commit (>=3.7.0,<4.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Description-Content-Type: text/markdown
 
 # DotConfig
 
 <a href="https://github.com/AidanInceer/DotDict">
-    <img alt="Static Badge" src="https://img.shields.io/badge/version-0.2.0-blue">
+    <img alt="Static Badge" src="https://img.shields.io/badge/version-0.3.0-blue">
 </a>
 
-A simple package which converts a standard python dictionary to a dot accessible object.
+A simple package which converts a standard python dictionary to a dot accessible configuration object.
 
 ## Installation
 
 ``` bash
 pip install dotcon
 ```
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: dotcon Version: 0.2.0 Summary: A simple package
+Metadata-Version: 2.1 Name: dotcon Version: 0.3.0 Summary: A simple package
 which converts a standard python dictionary to a dot accessible object.
 License: LICENCE Author: AidanInceer Author-email: aidaninceer0@gmail.com
 Requires-Python: >=3.11,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pre-commit (>=3.7.0,<4.0.0) Requires-Dist: pytest
 (>=8.1.1,<9.0.0) Description-Content-Type: text/markdown # DotConfig _[_S_t_a_t_i_c
 _B_a_d_g_e_]A simple package which converts a standard python dictionary to a dot
-accessible object. ## Installation ``` bash pip install dotcon ``` ## Usage ```
-python from dotcon import DotConfig mydict = { "A": [1, 2, 3, 4], "B": {"C":
-5}, "D": "E", "F": None, } ddict = DotConfig(mydict) ddict.A >>> [1, 2, 3, 4]
-ddict.B >>> {"C": 5} ddict.B.C >>> 5 ddict.D >>> "E" ddict.F >>> None ```
+accessible configuration object. ## Installation ``` bash pip install dotcon
+``` ## Usage ``` python from dotcon import DotConfig mydict = { "A": [1, 2, 3,
+4], "B": {"C": 5}, "D": "E", "F": None, } ddict = DotConfig(mydict) ddict.A >>>
+[1, 2, 3, 4] ddict.B >>> {"C": 5} ddict.B.C >>> 5 ddict.D >>> "E" ddict.F >>>
+None ```
```

