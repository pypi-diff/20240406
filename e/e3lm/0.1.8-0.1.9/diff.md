# Comparing `tmp/e3lm-0.1.8.tar.gz` & `tmp/e3lm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e3lm-0.1.8.tar", last modified: Fri Feb 10 18:39:25 2023, max compression
+gzip compressed data, was "e3lm-0.1.9.tar", last modified: Sat Apr  6 04:24:33 2024, max compression
```

## Comparing `e3lm-0.1.8.tar` & `e3lm-0.1.9.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 18:39:25.867379 e3lm-0.1.8/
--rw-rw-rw-   0        0        0     1089 2023-02-10 17:56:20.000000 e3lm-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     2997 2023-02-10 18:39:25.866378 e3lm-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2023-02-10 17:56:20.000000 e3lm-0.1.8/README.md
--rw-rw-rw-   0        0        0      104 2023-02-10 17:56:20.000000 e3lm-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-10 18:39:25.867379 e3lm-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1501 2023-02-10 18:38:46.000000 e3lm-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-10 18:39:25.823481 e3lm-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-02-10 18:39:25.831479 e3lm-0.1.8/src/e3lm/
--rw-rw-rw-   0        0        0       72 2021-10-08 23:05:35.000000 e3lm-0.1.8/src/e3lm/__init__.py
--rw-rw-rw-   0        0        0    28360 2023-02-10 18:38:44.000000 e3lm-0.1.8/src/e3lm/cli.py
-drwxrwxrwx   0        0        0        0 2023-02-10 18:39:25.846488 e3lm-0.1.8/src/e3lm/contrib/
--rw-rw-rw-   0        0        0        0 2021-10-08 22:11:33.000000 e3lm-0.1.8/src/e3lm/contrib/__init__.py
--rw-rw-rw-   0        0        0    14884 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/contrib/dot.py
--rw-rw-rw-   0        0        0     5722 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/contrib/json.py
--rw-rw-rw-   0        0        0     1043 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/contrib/ppt.py
--rw-rw-rw-   0        0        0     3769 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/contrib/units.py
-drwxrwxrwx   0        0        0        0 2023-02-10 18:39:25.848480 e3lm-0.1.8/src/e3lm/demos/
--rw-rw-rw-   0        0        0        0 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/demos/__init__.py
--rw-rw-rw-   0        0        0     7194 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/demos/data.py
-drwxrwxrwx   0        0        0        0 2023-02-10 18:39:25.849480 e3lm-0.1.8/src/e3lm/helpers/
--rw-rw-rw-   0        0        0        0 2021-10-08 22:11:33.000000 e3lm-0.1.8/src/e3lm/helpers/__init__.py
--rw-rw-rw-   0        0        0    11172 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/helpers/printers.py
-drwxrwxrwx   0        0        0        0 2023-02-10 18:39:25.855384 e3lm-0.1.8/src/e3lm/lang/
--rw-rw-rw-   0        0        0        0 2021-10-08 22:11:33.000000 e3lm-0.1.8/src/e3lm/lang/__init__.py
--rw-rw-rw-   0        0        0     7780 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/lang/ast.py
--rw-rw-rw-   0        0        0     1078 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/lang/data.py
--rw-rw-rw-   0        0        0    28587 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/lang/interpreters.py
--rw-rw-rw-   0        0        0    30482 2023-02-10 17:59:25.000000 e3lm-0.1.8/src/e3lm/lang/lexer.py
--rw-rw-rw-   0        0        0    13040 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/lang/parser.py
--rw-rw-rw-   0        0        0    14790 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/lang/parsetab.py
-drwxrwxrwx   0        0        0        0 2023-02-10 18:39:25.860578 e3lm-0.1.8/src/e3lm/tests/
--rw-rw-rw-   0        0        0        0 2021-10-08 22:11:33.000000 e3lm-0.1.8/src/e3lm/tests/__init__.py
--rw-rw-rw-   0        0        0     2618 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/tests/test_contrib.py
--rw-rw-rw-   0        0        0     1885 2021-10-08 22:11:33.000000 e3lm-0.1.8/src/e3lm/tests/test_interpreters.py
--rw-rw-rw-   0        0        0     1796 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/tests/test_lexer.py
--rw-rw-rw-   0        0        0     2206 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/tests/test_parser.py
--rw-rw-rw-   0        0        0      778 2021-10-08 22:11:33.000000 e3lm-0.1.8/src/e3lm/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-02-10 18:39:25.865378 e3lm-0.1.8/src/e3lm/utils/
--rw-rw-rw-   0        0        0        0 2021-10-08 22:11:33.000000 e3lm-0.1.8/src/e3lm/utils/__init__.py
--rw-rw-rw-   0        0        0      200 2021-10-08 22:11:33.000000 e3lm-0.1.8/src/e3lm/utils/funcs.py
--rw-rw-rw-   0        0        0     5259 2023-02-10 17:56:20.000000 e3lm-0.1.8/src/e3lm/utils/lang.py
--rw-rw-rw-   0        0        0      731 2021-10-08 22:11:33.000000 e3lm-0.1.8/src/e3lm/utils/spin.py
-drwxrwxrwx   0        0        0        0 2023-02-10 18:39:25.842480 e3lm-0.1.8/src/e3lm.egg-info/
--rw-rw-rw-   0        0        0     2997 2023-02-10 18:39:25.000000 e3lm-0.1.8/src/e3lm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-02-10 18:39:25.000000 e3lm-0.1.8/src/e3lm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 18:39:25.000000 e3lm-0.1.8/src/e3lm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-02-10 18:39:25.000000 e3lm-0.1.8/src/e3lm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      191 2023-02-10 18:39:25.000000 e3lm-0.1.8/src/e3lm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-02-10 18:39:25.000000 e3lm-0.1.8/src/e3lm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:33.585585 e3lm-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-06 04:24:29.000000 e3lm-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-06 04:24:33.585585 e3lm-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-06 04:24:29.000000 e3lm-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-06 04:24:29.000000 e3lm-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 04:24:33.585585 e3lm-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-06 04:24:29.000000 e3lm-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:33.577585 e3lm-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:33.581585 e3lm-0.1.9/src/e3lm/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27226 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:33.581585 e3lm-0.1.9/src/e3lm/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/contrib/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/contrib/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/contrib/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:33.581585 e3lm-0.1.9/src/e3lm/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/demos/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:33.581585 e3lm-0.1.9/src/e3lm/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/helpers/printers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:33.585585 e3lm-0.1.9/src/e3lm/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/lang/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/lang/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27778 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/lang/interpreters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29554 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/lang/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/lang/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14703 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/lang/parsetab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:33.585585 e3lm-0.1.9/src/e3lm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/tests/test_contrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/tests/test_interpreters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/tests/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:33.585585 e3lm-0.1.9/src/e3lm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/utils/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/utils/lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 04:24:29.000000 e3lm-0.1.9/src/e3lm/utils/spin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:24:33.585585 e3lm-0.1.9/src/e3lm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-06 04:24:33.000000 e3lm-0.1.9/src/e3lm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-06 04:24:33.000000 e3lm-0.1.9/src/e3lm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 04:24:33.000000 e3lm-0.1.9/src/e3lm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 04:24:33.000000 e3lm-0.1.9/src/e3lm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-06 04:24:33.000000 e3lm-0.1.9/src/e3lm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-06 04:24:33.000000 e3lm-0.1.9/src/e3lm.egg-info/top_level.txt
```

### Comparing `e3lm-0.1.8/LICENSE` & `e3lm-0.1.9/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Kenan Masri
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Kenan Masri
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `e3lm-0.1.8/PKG-INFO` & `e3lm-0.1.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,100 @@
-Metadata-Version: 2.1
-Name: e3lm
-Version: 0.1.8
-Summary: e3lm CLI tool (3lm language) for managing .3lm projects and files.
-Home-page: https://github.com/kenanmasri/3lm
-Author: Kenan Masri
-Author-email: kenanmasri@outlook.com
-Project-URL: Bug Tracker, https://github.com/kenanmasri/3lm/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<img src="https://i.ibb.co/gVczmTW/3LM.png" height="64" width="64" style="vertical-align: middle;"/> &nbsp;&nbsp; <span style="color: orange; font-size: 32px; vertical-align: middle;">3LM</span>
-
-<img src="https://img.shields.io/github/license/kenanmasri/3lm" /> <img src="https://img.shields.io/github/repo-size/kenanmasri/3lm" /> <img src="https://img.shields.io/pypi/v/e3lm" /> 
-
-Have fun while learning!
-
----
-
-## So what is this exactly?
-
-### This is an attempt at creating a markup language.
-
-3LM is a structure language parsed in Python.
-
-It is used for defining hierarchial objects, intended mainly to help write structured content fast and with ease.
-Whether you are a scientist, a programmer or an educator, 3LM can be useful for you.
-
-3LM is intended to be a language of use for an educational platform.
-
----
-
-<img src="https://i.ibb.co/5WQCkMW/screenshotto.png" alt="screenshotto" border="0">
-
----
-
-## Installation
-
-> NOTE: Installation does not work right now.. Since the package is not published to PyPI.
-
-### Installation from Github
-```bash
-$ pip install git+https://github.com/kenanmasri/3lm.git#egg=e3lm
-```
-
-### Installation through PyPI
-Creating a virtual environment is very preferrable.
-
-```bash
-$ python -m venv venv
-$ python -m pip install e3lm
-```
-
-## Configuration
-```env
-# Environment variables and their default values.
-
-E3LM_TEMP_DIRECTORY="tmp"
-```
-
-## Usage
-
-### Basic example
-
-You can run these in your terminal to make sure it works:
-
-```bash
-$ e3lm --version
-$ e3lm --help
-$ e3lm -d code0
-$ e3lm -d code0 -p json
-$ e3lm examples/lesson1
-```
-
-More examples:
-
-```bash
-# Interpret an example.3lm file.
-$ e3lm example.3lm
-
-# Interpret demo code1 and generate graphviz dot file and view graph image.
-$ e3lm -d code1 -p dot view
-
-# Benchmarking 20 times the demo code0 for 6 measurements.
-$ e3lm -d code0 -b 6 20
-```
-
----
-
-## Additional resources
-
-Refer to the [Wiki](https://github.com/kenanmasri/3lm/wiki) to learn the language.
-
----
-
-## TODO:
-
- - [ ] Examination questions auto-extraction from 3lm files. (Could be a plugin.)
- - [x] Rewrite included out-of-the-box example codes and error codes.
- - [ ] Add more tests.
- - [x] Benchmarking.
- - [x] Contrib plugins.
- - [ ] Make publish ready documentation.
- - [ ] Publish to PyPI.
-
-More possibilities... See [e3lm.todo](https://github.com/kenanmasri/3lm/blob/master/e3lm.todo)
-
----
+<img src="https://i.ibb.co/gVczmTW/3LM.png" height="64" width="64" style="vertical-align: middle;"/> &nbsp;&nbsp; <span style="color: orange; font-size: 32px; vertical-align: middle;">3LM</span>
+
+<img src="https://img.shields.io/github/license/knno/3lm" /> <img src="https://img.shields.io/github/repo-size/knno/3lm" /> <img src="https://img.shields.io/pypi/v/e3lm" /> 
+
+Have fun while learning!
+
+---
+
+## So what is this exactly?
+
+### This is an attempt at creating a markup language.
+
+3LM is a structure language parsed in Python.
+
+It is used for defining hierarchial objects, intended mainly to help write structured content fast and with ease.
+Whether you are a scientist, a programmer or an educator, 3LM can be useful for you.
+
+3LM is intended to be a language of use for an educational platform.
+
+---
+
+<img src="https://i.ibb.co/5WQCkMW/screenshotto.png" alt="screenshotto" border="0">
+
+---
+
+## Installation
+
+The recommended way to install is using PyPI
+
+### Installation through PyPI
+Creating a virtual environment is very preferrable.
+
+```bash
+$ python -m venv venv
+$ python -m pip install e3lm
+```
+
+### Installation from Github
+
+Not preferrable, but it works too :)
+
+```bash
+$ pip install git+https://github.com/knno/3lm.git#egg=e3lm
+```
+
+## Configuration
+```env
+# Environment variables and their default values.
+
+E3LM_TEMP_DIRECTORY="tmp"
+```
+
+## Usage
+
+### Basic example
+
+You can run these in your terminal to make sure it works:
+
+```bash
+$ e3lm --version
+$ e3lm --help
+$ e3lm -d code0
+$ e3lm -d code0 -p json
+$ e3lm examples/lesson1
+```
+
+More examples:
+
+```bash
+# Interpret an example.3lm file.
+$ e3lm example.3lm
+
+# Interpret demo code1 and generate graphviz dot file and view graph image.
+$ e3lm -d code1 -p dot view
+
+# Benchmarking 20 times the demo code0 for 6 measurements.
+$ e3lm -d code0 -b 6 20
+```
+
+---
+
+## Additional resources
+
+Refer to the [Wiki](https://github.com/knno/3lm/wiki) to learn the language.
+
+---
+
+## TODO:
+
+ - [ ] Examination questions auto-extraction from 3lm files. (Could be a plugin.)
+ - [x] Rewrite included out-of-the-box example codes and error codes.
+ - [ ] Add more tests.
+ - [x] Benchmarking.
+ - [x] Contrib plugins.
+ - [ ] Make publish ready documentation.
+ - [ ] Publish to PyPI.
+
+More possibilities... See [e3lm.todo](https://github.com/knno/3lm/blob/master/e3lm.todo)
+
+---
```

### Comparing `e3lm-0.1.8/setup.py` & `e3lm-0.1.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,55 @@
-#!/usr/bin/env python
-
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-install_requirements = [
-    "ansicolors",
-    "asciitree",
-    "attrs",
-    "graphviz",
-    "charset-normalizer",
-    "colorama",
-    "iniconfig",
-    "jinja2",
-    "lxml",
-    "markupsafe",
-    "more-itertools",
-    "packaging",
-    "pillow",
-    "pluggy",
-    "ply",
-    "py",
-    "pycodestyle",
-    "pyparsing",
-    "six",
-    "toml",
-    "tomli",
-    "untokenize",
-]
-
-if __name__ == "__main__":
-    setuptools.setup(
-        name="e3lm",
-        version="0.1.8",
-        author="Kenan Masri",
-        author_email="kenanmasri@outlook.com",
-        description="e3lm CLI tool (3lm language) for managing .3lm projects and files.",
-        long_description=long_description,
-        long_description_content_type="text/markdown",
-        url="https://github.com/kenanmasri/3lm",
-        project_urls={
-            "Bug Tracker": "https://github.com/kenanmasri/3lm/issues",
-        },
-        entry_points='''[console_scripts]\ne3lm=e3lm.cli:main''',
-        install_requires=install_requirements,
-        classifiers=[
-            "Programming Language :: Python :: 3",
-            "License :: OSI Approved :: MIT License",
-            "Operating System :: OS Independent",
-        ],
-        package_dir={"": "src"},
-        packages=setuptools.find_packages(where="src"),
-        python_requires=">=3.8",
-    )
+#!/usr/bin/env python
+
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+install_requirements = [
+    "ansicolors",
+    "asciitree",
+    "attrs",
+    "graphviz",
+    "charset-normalizer",
+    "colorama",
+    "iniconfig",
+    "jinja2",
+    "markupsafe",
+    "more-itertools",
+    "packaging",
+    "pillow",
+    "pluggy",
+    "ply",
+    "py",
+    "pycodestyle",
+    "pyparsing",
+    "six",
+    "toml",
+    "tomli",
+    "untokenize",
+]
+
+if __name__ == "__main__":
+    setuptools.setup(
+        name="e3lm",
+        version="0.1.9",
+        author="Kenan Masri",
+        author_email="kenanmasri@outlook.com",
+        description="e3lm CLI tool (3lm language) for managing .3lm projects and files.",
+        long_description=long_description,
+        long_description_content_type="text/markdown",
+        url="https://github.com/knno/3lm",
+        project_urls={
+            "Bug Tracker": "https://github.com/knno/3lm/issues",
+        },
+        entry_points='''[console_scripts]\ne3lm=e3lm.cli:main''',
+        install_requires=install_requirements,
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "License :: OSI Approved :: MIT License",
+            "Operating System :: OS Independent",
+        ],
+        package_dir={"": "src"},
+        packages=setuptools.find_packages(where="src"),
+        python_requires=">=3.8",
+    )
```

### Comparing `e3lm-0.1.8/src/e3lm/cli.py` & `e3lm-0.1.9/src/e3lm/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,695 +1,686 @@
-# -*- coding: utf-8 -*-
-"""The e3lm CLI tool (3lm language) for managing 3lm projects and files.
-
-This tool is designed mainly to enable interpretation of 3lm files and
-upgrading the interpreter and its plugins.
-"""
-__version__ = "0.1.8"
-
-__doc2__ = """additional arguments:
-    Nothing for now.
-"""
-
-__doc3__ = """additional arguments:
-  --plugin-list         view available plugins, use the following command:
-  --plugin-install plugin
-                        install a specific plugin
-  --plugin-update plugin
-                        update a specific plugin
-  --plugin-uninstall plugin
-                        uninstall a specific plugin
-  --clear-cache         clear the temporary files cache
-  --lang-update         check for language updates
-"""
-
-import argparse
-import io
-import itertools
-import json
-import os
-import signal
-import subprocess
-import sys
-import textwrap
-import timeit
-from datetime import datetime
-from shlex import quote
-from time import perf_counter, sleep
-
-from graphviz import Source as GraphvizSource
-
-from e3lm.contrib.dot import DotPlugin as Dot
-from e3lm.contrib.json import JsonPlugin as Json
-from e3lm.demos.data import getcode as gettestcode
-from e3lm.helpers import printers
-from e3lm.helpers.printers import COLORS
-from e3lm.lang.ast import basic_dt
-from e3lm.lang.interpreters import E3lmInterpreter, E3lmPlugin
-from e3lm.utils.lang import get_plugin, interpret, lex, parse
-from e3lm.utils.spin import animate as spinner
-
-# Variables
-
-CLI_PLUGINS = [
-    "view",
-    "lex",
-    "parse",
-]  # Plugins that are not E3lmPlugin
-
-
-def windows_enable_ANSI(std_id):
-    """Enable Windows 10 cmd.exe ANSI VT Virtual Terminal Processing."""
-    from ctypes import POINTER, WINFUNCTYPE, byref, windll
-    from ctypes.wintypes import BOOL, DWORD, HANDLE
-
-    GetStdHandle = WINFUNCTYPE(
-        HANDLE,
-        DWORD)(('GetStdHandle', windll.kernel32))
-
-    GetFileType = WINFUNCTYPE(
-        DWORD,
-        HANDLE)(('GetFileType', windll.kernel32))
-
-    GetConsoleMode = WINFUNCTYPE(
-        BOOL,
-        HANDLE,
-        POINTER(DWORD))(('GetConsoleMode', windll.kernel32))
-
-    SetConsoleMode = WINFUNCTYPE(
-        BOOL,
-        HANDLE,
-        DWORD)(('SetConsoleMode', windll.kernel32))
-
-    if std_id == 1:       # stdout
-        h = GetStdHandle(-11)
-    elif std_id == 2:     # stderr
-        h = GetStdHandle(-12)
-    else:
-        return False
-
-    if h is None or h == HANDLE(-1):
-        return False
-
-    FILE_TYPE_CHAR = 0x0002
-    if (GetFileType(h) & 3) != FILE_TYPE_CHAR:
-        return False
-
-    mode = DWORD()
-    if not GetConsoleMode(h, byref(mode)):
-        return False
-
-    ENABLE_VIRTUAL_TERMINAL_PROCESSING = 0x0004
-    if (mode.value & ENABLE_VIRTUAL_TERMINAL_PROCESSING) == 0:
-        SetConsoleMode(h, mode.value | ENABLE_VIRTUAL_TERMINAL_PROCESSING)
-    return True
-
-
-if sys.platform == "win32":
-    windows_enable_ANSI(0)  # Windows 10 VirtualTerminal Ansi on Stdout
-    windows_enable_ANSI(1)  # Windows 10 VirtualTerminal Ansi on Stderr
-
-sys.stdout.reconfigure(encoding='utf-8')
-sys.stderr.reconfigure(encoding='utf-8')
-
-# E3lm CLI
-
-
-def arg_required_length(nmin, nmax):
-    class RequiredLength(argparse.Action):
-        def __call__(self, parser, args, values, option_string=None):
-            if not nmin <= len(values) <= nmax:
-                msg = 'argument "{f}" requires between {nmin} and {nmax} arguments'.format(
-                    f=self.dest, nmin=nmin, nmax=nmax)
-                raise argparse.ArgumentTypeError(msg)
-            setattr(args, self.dest, values)
-    return RequiredLength
-
-
-def demo_file(f):
-    if f.startswith("code"):
-        n = int(f[4:])
-        prefix = "code"
-    elif f.startswith("errorcode"):
-        n = int(f[9:])
-        prefix = "errorcode"
-    else:
-        n = int(f)
-    return gettestcode(n, prefix)
-    # return "<<..demo file " + str(f) + "..>>"
-
-
-def demo_exists(f):
-    return demo_file(f) != None
-
-
-def CLI(input_file="-", kwargs={}):
-    """The actual CLI."""
-    if kwargs:
-        quiet = kwargs["quiet"]
-        verbose = kwargs["verbose"]
-        verbose_lvl = kwargs["verbose_lvl"]
-        demos = kwargs["demos"]
-        plugins = kwargs["plugins"]
-        nocolors = kwargs["nocolors"]
-        noglyph = kwargs["noglyph"]
-        formatstyle = kwargs["formatstyle"]
-        benchmarking = kwargs["benchmarking"]
-        benchmarking_mods = kwargs["benchmarking_mods"]
-        colors = kwargs["colors"]
-
-    shown_msgs = {}
-    runstack = {}
-    runtime = {}
-    special_positionals = ("?", "help",  # Help alternatives.
-                           "-", ".",  # No or all file(s)
-                           )
-
-    tmpdir = os.getenv("E3LM_TEMP_DIRECTORY", "tmp")
-    if not os.path.exists(tmpdir):
-        os.mkdir(tmpdir)
-
-    # Check for special positional argument values in place of "file"
-    if input_file in special_positionals:
-        if input_file in ["?", "help"]:
-            sys.exit(e3lm_parser.print_help(None))
-        elif input_file in ["-", "."]:
-            if input_file == "-":
-                input_file = None
-            else:
-                runstack.update({os.path.basename(f): os.path.abspath(f)
-                                for f in os.listdir(os.getcwd()) if f.endswith(".3lm")})
-                input_file = None
-
-    # Check if file exists... otherwise use demos.
-    if input_file != None:
-        if (os.path.exists(input_file) or os.path.exists(input_file + ".3lm")) \
-                and (os.path.isfile(input_file) or os.path.isfile(input_file + ".3lm")):
-            if not input_file.endswith(".3lm"):
-                input_file = input_file + ".3lm"
-            runstack.update({input_file: input_file})
-        else:
-            if not input_file.endswith(".3lm"):
-                input_file = input_file + ".3lm"
-            if not os.path.isfile(input_file):
-                # if not quiet:
-                print(colors["E"] + 'Error: ' + input_file +
-                      ' does not exist.' + colors["R"], file=sys.stderr)
-            # elif not quiet:
-            else:
-                print(colors["E"] + 'Error: ' + input_file +
-                      ' is a directory.' + colors["R"], file=sys.stderr)
-            sys.exit(1)
-
-    # Check if demos are specified
-    if len(demos) > 0:
-        runstack.update({d: demo_file(d) for d in demos if demo_exists(d)})
-
-    # Load up each stack content (file or directly)
-    for key, val in runstack.items():
-        if os.path.isfile(val) and os.path.exists(val):
-            try:
-                f = open(val, encoding='utf-8')
-                d = "".join(f.readlines())
-                if benchmarking_mods["enabled"]:
-                    d = (d + "\n") * int(benchmarking_mods["lengthofcode"])
-                    runstack[key] = d
-                runstack[key] = d
-            finally:
-                f.close()
-        else:
-            d = val
-            if benchmarking_mods["enabled"]:
-                d = (d + "\n") * int(benchmarking_mods["lengthofcode"])
-            runstack[key] = d
-
-    # Print headers for each runtime
-    for i, run in runstack.items():
-        if formatstyle == "DEFAULT":
-            printers.cprint(colors["3"] + "--" + colors["1"] + "== " + colors["4"] +
-                            i + colors["1"] + " ==" + colors["3"] + "--" + colors["R"], color="" if nocolors else "SUCCESS")
-        elif formatstyle == "MIN":
-            pass
-        elif formatstyle == "COMPATIBLE":
-            print("Runtime.begin", i)
-
-        run_plugins = [get_plugin(p) for p in plugins if p not in CLI_PLUGINS and
-                       type(get_plugin(p)) not in basic_dt]
-
-        if "lex" in plugins:
-            run_program = lex(run, i, debug=verbose_lvl >= 2,
-                              enable_colors=nocolors == False, tracking=verbose_lvl >= 2)
-            return True
-
-        if "parse" in plugins:
-            run_program = parse(run, i, parser_kwargs={
-                "tracking": verbose_lvl >= 2,
-                "enable_colors": nocolors == False,
-                "debug": verbose_lvl >= 2,
-            }, debug=verbose_lvl >= 3)
-            if verbose_lvl >= 2:
-                if not benchmarking_mods["enabled"]:
-                    if formatstyle == "COMPATIBLE":
-                        print("Program.begin", i)
-                    printers.nprint(run_program, max_level=0, pallete=None if nocolors else COLORS,
-                                    noglyph=noglyph, program_name=i, evaluate=False)
-                    if formatstyle == "COMPATIBLE":
-                        print("Program.end")
-
-                else:
-                    if "benchmarking_parse" not in shown_msgs.keys():
-                        count = str(len(run.splitlines()))
-                        shown_msgs["benchmarking_parse"] = True
-                        if formatstyle == "DEFAULT":
-                            print(colors["2"] + "       - " + colors["H"] +
-                                  count + " line(s) of code Total." + colors["R"])
-                        elif formatstyle == "COMPATIBLE":
-                            print("Benchmark.info:", count)
-
-        run_program = interpret(run, i,
-                                plugins=run_plugins,
-                                debug=verbose_lvl >= 3, enable_colors=nocolors == False,
-                                parser_kwargs={
-                                    "tracking": verbose_lvl >= 2,
-                                    "enable_colors": True,
-                                    "debug": verbose_lvl >= 3,
-                                }
-                                )
-        if verbose_lvl >= 2:
-            if not benchmarking_mods["enabled"]:
-                if formatstyle == "COMPATIBLE":
-                    print("Program.begin", i)
-                printers.nprint(run_program, max_level=0, pallete=None if nocolors else COLORS,
-                                noglyph=noglyph, program_name=i, evaluate=True)
-                if formatstyle == "COMPATIBLE":
-                    print("Program.end")
-            else:
-                if "benchmarking_parse" not in shown_msgs.keys():
-                    count = str(len(run.splitlines()))
-                    shown_msgs["benchmarking_parse"] = True
-                    if formatstyle == "DEFAULT":
-                        print(colors["2"] + "       - " + colors["H"] +
-                              count + " line(s) of code Total." + colors["R"])
-                    elif formatstyle == "COMPATIBLE":
-                        print("Benchmark.info.loc_count", count)
-
-                if "benchmarking_intr" not in shown_msgs.keys():
-                    count = str(len(run_program.flat_blocks))
-                    shown_msgs["benchmarking_intr"] = True
-                    if formatstyle == "DEFAULT":
-                        print(colors["2"] + "       - " + colors["H"] +
-                              count + " blocks(s) Total." + colors["R"])
-                    elif formatstyle == "COMPATIBLE":
-                        print("Benchmark.info.block_count", count)
-
-        if "benchmarking_parse" in shown_msgs.keys():
-            del shown_msgs["benchmarking_parse"]
-        if "benchmarking_intr" in shown_msgs.keys():
-            del shown_msgs["benchmarking_intr"]
-
-        if run_program == None:
-            print("None")
-        if "json" in plugins:
-            if formatstyle == "COMPATIBLE":
-                print("Plugin.json.begin")
-            print(json.dumps(run_program.json, indent=4))
-            if formatstyle == "COMPATIBLE":
-                print("Plugin.json.end")
-
-        if "view" in plugins:
-            if run_program:
-                if not hasattr(run_program, "dot_source"):
-                    if formatstyle == "DEFAULT":
-                        print(
-                            colors["E"] + 'Error: Program does not have dot_source.' + colors["R"], file=sys.stderr)
-                    elif formatstyle == "COMPATIBLE":
-                        print("Plugin.view.error",
-                              "Program does not have dot_source.")
-                    exit(1)
-
-                if formatstyle == "DEFAULT":
-                    graph = GraphvizSource(
-                        run_program.dot_source, filename=tmpdir + "/" + i + ".dot", format="png")
-                    graph.view()
-                elif formatstyle == "COMPATIBLE":
-                    print("Plugin.dot.begin")
-                    print(run_program.dot_source)
-                    print("Plugin.dot.end")
-            else:
-                if formatstyle == "DEFAULT":
-                    print("Nothing to view")
-                elif formatstyle == "COMPATIBLE":
-                    print("Plugin.view.info", "Nothing to view")
-
-    sys.exit(0)
-
-
-def caller(the_call, _type="subprocess", shell=True, ret=False, stdout=-1, stderr=-1):
-    """Calls a shell command, or a program."""
-
-    if _type == "os":
-        proc = subprocess.Popen(the_call,
-                                shell=shell,
-                                stdout=stdout,
-                                bufsize=-1,
-                                stderr=stderr,
-                                # preexec_fn=os.setsid
-                                )
-        if ret:
-            return proc
-        try:
-            p = os._wrap_close(io.TextIOWrapper(proc.stdout), proc)
-            return p.read()
-        except KeyboardInterrupt:
-            os.killpg(os.getpgid(proc.pid), signal.SIGTERM)
-            return False
-
-    elif _type == "subprocess":
-        p = subprocess.Popen(the_call, shell=shell,
-                             stderr=stderr, stdout=stdout)
-        return p
-
-
-def BENCHMARK(input_file, kwargs={}):
-    import math
-
-    if kwargs:
-        quiet = kwargs["quiet"]
-        verbose = kwargs["verbose"]
-        verbose_lvl = kwargs["verbose_lvl"]
-        demos = kwargs["demos"]
-        plugins = kwargs["plugins"]
-        nocolors = kwargs["nocolors"]
-        noglyph = kwargs["noglyph"]
-        formatstyle = kwargs["formatstyle"]
-        benchmarking = kwargs["benchmarking"]
-        benchmarking_mods = kwargs["benchmarking_mods"]
-        colors = kwargs["colors"]
-
-    shown_msgs = {}
-    py = "python"
-    if formatstyle == "DEFAULT":
-        printers.cprint(colors["2"] + "--" + colors["2"] + "== " + colors["2"] +
-                        "Benchmarking..." + colors["2"] + " ==" + colors["2"] + "--" + colors["R"], color="" if nocolors else "SUCCESS")
-    elif formatstyle == "COMPATIBLE":
-        print("Benchmark.begin")
-
-    sys_argv_ = sys.argv
-    sys_argv_.pop(0)
-    sys_argv_.append("--benchmark-mods")
-    sys_argv_.append(
-        "lengthofcode=" + str(benchmarking[1]) + "," +
-        "iterations=" + str(benchmarking[0]) + ""
-    )
-
-    iterations = 0
-    err_count = 0
-    timelog = []
-
-    while iterations < int(benchmarking[0]):
-        # Open a subprocess for running the wanted command...
-        try:
-            # Remove the benchmark arguments and pass the rest to the caller.
-            strings = sys_argv_
-            for string in strings:
-                if string == "-b" or string == "--benchmark":
-                    pos = strings.index(string) + 1
-                    if benchmarking[0] != 0:
-                        if benchmarking[0] == strings[pos]:
-                            strings.pop(pos)
-                            pos -= 1
-                    if benchmarking[1] != 0:
-                        if benchmarking[1] == strings[pos + 1]:
-                            strings.pop(pos + 1)
-                            pos -= 1
-                    strings.remove(string)
-                    break
-
-            call = " ".join([quote(s) for s in strings])
-            if verbose_lvl == 3:
-                if "dbg_benchmark_init" not in shown_msgs.keys():
-                    print(colors["BLUE"] + "DBG: The call in subprocess is: " +
-                          colors["CYAN"] + "python e3lm.py " + call)
-            p = caller("\"" + py + "\"" + " " + "\"" + os.path.abspath(__file__) +
-                       "\" " + call, _type="subprocess", shell=False, ret=True)
-            pout = os._wrap_close(io.TextIOWrapper(p.stdout), p)
-            perr = os._wrap_close(io.TextIOWrapper(p.stderr), p)
-
-            t_start = perf_counter()
-            read_total_perr = ""
-            read_total_pout = ""
-            for c in itertools.cycle([
-                '⡀', '⠄', '⠂', '⠁', '⠈', '⠐', '⠠', '⢀',
-            ]):
-                if "benchmark_first_iteration" not in shown_msgs.keys():
-                    read_pout = pout.read()
-                    read_perr = perr.read()
-                    read_total_pout = read_total_pout + "\n" + read_pout
-                    read_total_perr = read_total_perr + "\n" + read_perr
-                    if read_pout != "":
-                        if formatstyle == "DEFAULT":
-                            print(colors["2"] + "       OUT: " +
-                                  colors["R"] + read_pout)
-                        elif formatstyle == "COMPATIBLE":
-                            print("Benchmark.out", read_pout)
-                    if read_perr != "":
-                        if formatstyle == "DEFAULT":
-                            print(colors["E"] + "       ERR: " +
-                                  colors["R"] + read_perr)
-                        elif formatstyle == "COMPATIBLE":
-                            print("Benchmark.err", read_perr)
-                        raise TimeoutError("An error occured, aborting..")
-                if p.poll() != None:
-                    shown_msgs["benchmark_first_iteration"] = True
-                    break
-                else:
-                    if formatstyle == "DEFAULT":
-                        sys.stdout.write('\r' + c + ' ' +
-                                         "inst: " + str(iterations) + "  ")
-                        sys.stdout.flush()
-                    sleep(0.033)
-            t_end = perf_counter()
-        except KeyboardInterrupt:
-            if formatstyle == "DEFAULT":
-                print(colors["GREEN"] +
-                      "\nUser cancelled (KeyboardInterrupt)" + colors["R"])
-                printers.cprint(colors["2"] + "--" + colors["2"] + "== " + colors["2"] +
-                                "Benchmarking done..." + colors["2"] + " ==" + colors["2"] + "--" + colors["R"] + "\n", color="" if nocolors else "SUCCESS")
-            elif formatstyle == "COMPATIBLE":
-                print("Benchmark.cancelled")
-                print("Benchmark.end")
-
-            exit(0)
-        except TimeoutError as e:
-            if formatstyle == "DEFAULT":
-                print(colors["GREEN"] + "Timeout: " + str(e) + colors["R"])
-                printers.cprint(colors["2"] + "--" + colors["2"] + "== " + colors["2"] +
-                                "Benchmarking done..." + colors["2"] + " ==" + colors["2"] + "--" + colors["R"] + "\n", color="" if nocolors else "SUCCESS")
-            elif formatstyle == "COMPATIBLE":
-                print("Benchmark.timeout", str(e))
-                print("Benchmark.end")
-            exit(1)
-
-        timelog.append({
-            "iteration": iterations,
-            "start": t_start,
-            "end": t_end,
-            "stdout": read_total_pout,
-            "stderr": read_total_perr,
-        })
-
-        shown_msgs["dbg_benchmark_init"] = True
-        iterations += 1
-
-    if formatstyle == "DEFAULT":
-        sys.stdout.write('\r' + 'Total iterations: ' + str(iterations) + '\n')
-    elif formatstyle == "COMPATIBLE":
-        sys.stdout.write('Benchmark.info.total_iter ' + str(iterations) + '\n')
-    sys.stdout.flush()
-
-    if formatstyle == "DEFAULT":
-        [print(str(t["iteration"]) + " => " + str(round((t["end"] - t["start"]) *
-                                                        1000, 1000))[:6] + " ms") for t in timelog]
-    elif formatstyle == "COMPATIBLE":
-        [print("Benchmark.info.iter", str(t["iteration"]) + " " + str(round((t["end"] - t["start"]) *
-                                                                            1000, 1000))[:6] + " ms") for t in timelog]
-
-    durations = [t["end"] - t["start"] for t in timelog]
-    if formatstyle == "DEFAULT":
-        print(colors["1"] + "Max: " + colors["HEADER"] + str(round((max(durations)) *
-                                                                   1000, 1000))[:6] + colors["1"] + " ms" + colors["R"])
-        print(colors["1"] + "Min: " + colors["HEADER"] + str(round((min(durations)) *
-                                                                   1000, 1000))[:6] + colors["1"] + " ms" + colors["R"])
-        print(colors["1"] + "Avg: " + colors["HEADER"] + str(round((sum(durations) /
-                                                                    iterations) * 1000, 1000))[:6] + colors["1"] + " ms" + colors["R"])
-        printers.cprint(colors["2"] + "--" + colors["2"] + "== " + colors["2"] +
-                        "Benchmarking done..." + colors["2"] + " ==" + colors["2"] + "--" + colors["R"] + "\n", color="" if nocolors else "SUCCESS")
-    elif formatstyle == "COMPATIBLE":
-        print("Benchmark.info.max", str(round((max(durations)) *
-                                              1000, 1000))[:6])
-        print("Benchmark.info.min", str(round((min(durations)) *
-                                              1000, 1000))[:6])
-        print("Benchmark.info.avg", str(round((sum(durations) /
-                                               iterations) * 1000, 1000))[:6])
-        print("Benchmark.end")
-
-    exit(0)
-
-
-def main():
-    e3lm_parser = argparse.ArgumentParser(prog='e3lm',
-                                          usage='%(prog)s [options] file',
-                                          description=__doc__,
-                                          formatter_class=argparse.RawTextHelpFormatter,
-                                          epilog=__doc2__)
-
-    e3lm_parser.add_argument('--version', action="version",
-                             version="e3lm CLI v" + __version__ + " (3lm language)")
-
-    e3lm_parser.add_argument('file',
-                             nargs='?',
-                             default='-',
-                             help='path to the 3lm file (automatically detects extension) or - for nothing',
-                             )
-
-    e3lm_parser.add_argument('-q',
-                             '--quiet',
-                             action='store_true',
-                             dest='quiet',
-                             default=False,
-                             help='run quietly without any output')
-
-    e3lm_parser.add_argument('-nc',
-                             '--no-color',
-                             action='store_true',
-                             dest="nocolors",
-                             default=False,
-                             help='set output to be without ANSI colors')
-
-    e3lm_parser.add_argument('-ng',
-                             '--no-glyph',
-                             action='store_true',
-                             dest="noglyph",
-                             default=False,
-                             help='use non-glyph character to avoid encoding issues')
-
-    e3lm_parser.add_argument('-v',
-                             '--verbose',
-                             action='store',
-                             metavar='NONE|ERROR|INFO|DEBUG',
-                             dest='verbose',
-                             type=str,
-                             choices=["NONE", "ERROR", "INFO", "DEBUG"],
-                             default="INFO",
-                             help='filter output messages (default is INFO)')
-
-    # e3lm_parser.add_argument('-i',
-    #                          '--interactive',
-    #                          action='store_true',
-    #                          default=False,
-    #                          help='execute with interactive mode')
-
-    e3lm_parser.add_argument('-p',
-                             '--plugin',
-                             action='store',
-                             metavar='plugin',
-                             type=str,
-                             default="",
-                             nargs="+",
-                             help='interpret using plugin(s). see below')
-
-    e3lm_parser.add_argument('-d',
-                             '--demo',
-                             dest='demo',
-                             metavar="code<n>",
-                             action='store',
-                             nargs='+',
-                             type=str,
-                             help='interpret demos in addition'
-                             )
-
-    e3lm_parser.add_argument('-b',
-                             '--benchmark',
-                             metavar='N',
-                             dest='benchmarking',
-                             default=False,
-                             action=arg_required_length(0, 2),
-                             nargs="*",
-                             help="Benchmark N number of times [and N times length of code]",
-                             )
-
-    e3lm_parser.add_argument('-fs',
-                             '--formatstyle',
-                             action='store',
-                             metavar='DEFAULT|MIN|COMPATIBLE',
-                             dest='formatstyle',
-                             type=str,
-                             choices=["DEFAULT", "MIN", "COMPATIBLE"],
-                             default="DEFAULT",
-                             help='Formatting of the output messages',
-                             )
-
-    # For passing BENCHMARK to subprocess to modify length of codes.
-    e3lm_parser.add_argument('--benchmark-mods',
-                             dest='benchmarking_mods',
-                             required=False, type=str,
-                             help=argparse.SUPPRESS)
-
-    args = e3lm_parser.parse_args()
-
-    quiet = args.quiet
-    if quiet:
-        verbose = "NONE"
-    verbose = args.verbose.upper()
-    verbose_lvl = 1 if verbose == "ERROR" else 2 if verbose == "INFO" else 3 if verbose == "DEBUG" else 0
-    input_file = args.file
-    demos = args.demo or []
-    plugins = args.plugin or []
-    nocolors = args.nocolors
-    noglyph = args.noglyph
-    formatstyle = args.formatstyle
-
-    colors = COLORS
-    if nocolors:
-        colors = {k: "" for k in COLORS.keys()}
-    benchmarking = args.benchmarking
-    benchmarking_mods = args.benchmarking_mods
-    if benchmarking_mods == None:
-        benchmarking_mods = {}
-        benchmarking_mods["enabled"] = False
-    else:
-        benchmarking_mods = benchmarking_mods.split(",")
-        benchmarking_mods = {b.split('=')[0]: b.split(
-            '=')[1] for b in benchmarking_mods}
-        benchmarking_mods["enabled"] = True
-
-    kwargs = {
-        "args": args,
-        "quiet": quiet,
-        "verbose": verbose,
-        "verbose_lvl": verbose_lvl,
-        "demos": demos,
-        "plugins": plugins,
-        "nocolors": nocolors,
-        "noglyph": noglyph,
-        "formatstyle": formatstyle,
-        "benchmarking": benchmarking,
-        "benchmarking_mods": benchmarking_mods,
-        "colors": colors,
-    }
-
-    # --- Check if benchmarking ---
-    if benchmarking != False:
-        if type(benchmarking) == list:
-            if len(benchmarking) == 0:
-                benchmarking = [1, 1, ]
-            elif len(benchmarking) == 1:
-                benchmarking.append(1)
-        if benchmarking[0] != 0 and benchmarking[1] != 0:
-            BENCHMARK(input_file, kwargs=kwargs)
-    else:
-        # --- Actual program ---
-        CLI(input_file, kwargs=kwargs)
-
-
-if __name__ == "__main__":
-    main()
+# -*- coding: utf-8 -*-
+"""The e3lm CLI tool (3lm language) for managing 3lm projects and files.
+
+This tool is designed mainly to enable interpretation of 3lm files and
+upgrading the interpreter and its plugins.
+"""
+__version__ = "0.1.9"
+
+__doc2__ = """additional arguments:
+    Nothing for now.
+"""
+
+__doc3__ = """additional arguments:
+  --plugin-list         view available plugins, use the following command:
+  --plugin-install plugin
+                        install a specific plugin
+  --plugin-update plugin
+                        update a specific plugin
+  --plugin-uninstall plugin
+                        uninstall a specific plugin
+  --clear-cache         clear the temporary files cache
+  --lang-update         check for language updates
+"""
+
+import argparse
+import io
+import itertools
+import json
+import os
+import signal
+import subprocess
+import sys
+from shlex import quote
+from time import perf_counter, sleep
+
+from graphviz import Source as GraphvizSource
+
+from e3lm.contrib.dot import DotPlugin as Dot
+from e3lm.contrib.json import JsonPlugin as Json
+from e3lm.demos.data import getcode as gettestcode
+from e3lm.helpers import printers
+from e3lm.helpers.printers import COLORS
+from e3lm.lang.ast import basic_dt
+from e3lm.lang.interpreters import E3lmInterpreter, E3lmPlugin
+from e3lm.utils.lang import get_plugin, interpret, lex, parse
+
+# Variables
+
+CLI_PLUGINS = [
+    "view",
+    "lex",
+    "parse",
+]  # Plugins that are not E3lmPlugin
+
+
+def windows_enable_ANSI(std_id):
+    """Enable Windows 10 cmd.exe ANSI VT Virtual Terminal Processing."""
+    from ctypes import POINTER, WINFUNCTYPE, byref, windll
+    from ctypes.wintypes import BOOL, DWORD, HANDLE
+
+    GetStdHandle = WINFUNCTYPE(
+        HANDLE,
+        DWORD)(('GetStdHandle', windll.kernel32))
+
+    GetFileType = WINFUNCTYPE(
+        DWORD,
+        HANDLE)(('GetFileType', windll.kernel32))
+
+    GetConsoleMode = WINFUNCTYPE(
+        BOOL,
+        HANDLE,
+        POINTER(DWORD))(('GetConsoleMode', windll.kernel32))
+
+    SetConsoleMode = WINFUNCTYPE(
+        BOOL,
+        HANDLE,
+        DWORD)(('SetConsoleMode', windll.kernel32))
+
+    if std_id == 1:       # stdout
+        h = GetStdHandle(-11)
+    elif std_id == 2:     # stderr
+        h = GetStdHandle(-12)
+    else:
+        return False
+
+    if h is None or h == HANDLE(-1):
+        return False
+
+    FILE_TYPE_CHAR = 0x0002
+    if (GetFileType(h) & 3) != FILE_TYPE_CHAR:
+        return False
+
+    mode = DWORD()
+    if not GetConsoleMode(h, byref(mode)):
+        return False
+
+    ENABLE_VIRTUAL_TERMINAL_PROCESSING = 0x0004
+    if (mode.value & ENABLE_VIRTUAL_TERMINAL_PROCESSING) == 0:
+        SetConsoleMode(h, mode.value | ENABLE_VIRTUAL_TERMINAL_PROCESSING)
+    return True
+
+
+if sys.platform == "win32":
+    windows_enable_ANSI(0)  # Windows 10 VirtualTerminal Ansi on Stdout
+    windows_enable_ANSI(1)  # Windows 10 VirtualTerminal Ansi on Stderr
+
+sys.stdout.reconfigure(encoding='utf-8')
+sys.stderr.reconfigure(encoding='utf-8')
+
+# E3lm CLI
+
+
+def arg_required_length(nmin, nmax):
+    class RequiredLength(argparse.Action):
+        def __call__(self, parser, args, values, option_string=None):
+            if not nmin <= len(values) <= nmax:
+                msg = 'argument "{f}" requires between {nmin} and {nmax} arguments'.format(
+                    f=self.dest, nmin=nmin, nmax=nmax)
+                raise argparse.ArgumentTypeError(msg)
+            setattr(args, self.dest, values)
+    return RequiredLength
+
+
+def demo_file(f):
+    if f.startswith("code"):
+        n = int(f[4:])
+        prefix = "code"
+    elif f.startswith("errorcode"):
+        n = int(f[9:])
+        prefix = "errorcode"
+    else:
+        n = int(f)
+    return gettestcode(n, prefix)
+    # return "<<..demo file " + str(f) + "..>>"
+
+
+def demo_exists(f):
+    return demo_file(f) != None
+
+
+def CLI(input_file="-", kwargs={}):
+    """The actual CLI."""
+    if kwargs:
+        quiet = kwargs["quiet"]
+        verbose = kwargs["verbose"]
+        verbose_lvl = kwargs["verbose_lvl"]
+        demos = kwargs["demos"]
+        plugins = kwargs["plugins"]
+        nocolors = kwargs["nocolors"]
+        noglyph = kwargs["noglyph"]
+        formatstyle = kwargs["formatstyle"]
+        benchmarking = kwargs["benchmarking"]
+        benchmarking_mods = kwargs["benchmarking_mods"]
+        colors = kwargs["colors"]
+        e3lm_parser = kwargs["e3lm_parser"]
+
+    shown_msgs = {}
+    runstack = {}
+    runtime = {}
+    special_positionals = ("?", "help",  # Help alternatives.
+                           "-", ".",  # No or all file(s)
+                           )
+
+    tmpdir = os.getenv("E3LM_TEMP_DIRECTORY", "tmp")
+    if not os.path.exists(tmpdir):
+        os.mkdir(tmpdir)
+
+    # Check for special positional argument values in place of "file"
+    if input_file in special_positionals:
+        if input_file in ["?", "help"]:
+            sys.exit(e3lm_parser.print_help(None))
+        elif input_file in ["-", "."]:
+            if input_file == "-":
+                input_file = None
+            else:
+                runstack.update({os.path.basename(f): os.path.abspath(f)
+                                for f in os.listdir(os.getcwd()) if f.endswith(".3lm")})
+                input_file = None
+
+    # Check if file exists... otherwise use demos.
+    if input_file != None:
+        if (os.path.exists(input_file) or os.path.exists(input_file + ".3lm")) \
+                and (os.path.isfile(input_file) or os.path.isfile(input_file + ".3lm")):
+            if not input_file.endswith(".3lm"):
+                input_file = input_file + ".3lm"
+            runstack.update({input_file: input_file})
+        else:
+            if not input_file.endswith(".3lm"):
+                input_file = input_file + ".3lm"
+            if not os.path.isfile(input_file):
+                # if not quiet:
+                print(colors["E"] + 'Error: ' + input_file +
+                      ' does not exist.' + colors["R"], file=sys.stderr)
+            # elif not quiet:
+            else:
+                print(colors["E"] + 'Error: ' + input_file +
+                      ' is a directory.' + colors["R"], file=sys.stderr)
+            sys.exit(1)
+
+    # Check if demos are specified
+    if len(demos) > 0:
+        runstack.update({d: demo_file(d) for d in demos if demo_exists(d)})
+
+    # Load up each stack content (file or directly)
+    for key, val in runstack.items():
+        if os.path.isfile(val) and os.path.exists(val):
+            try:
+                f = open(val, encoding='utf-8')
+                d = "".join(f.readlines())
+                if benchmarking_mods["enabled"]:
+                    d = (d + "\n") * int(benchmarking_mods["lengthofcode"])
+                    runstack[key] = d
+                runstack[key] = d
+            finally:
+                f.close()
+        else:
+            d = val
+            if benchmarking_mods["enabled"]:
+                d = (d + "\n") * int(benchmarking_mods["lengthofcode"])
+            runstack[key] = d
+
+    # Print headers for each runtime
+    for i, run in runstack.items():
+        if formatstyle == "DEFAULT":
+            printers.cprint(colors["3"] + "--" + colors["1"] + "== " + colors["4"] +
+                            i + colors["1"] + " ==" + colors["3"] + "--" + colors["R"], color="" if nocolors else "SUCCESS")
+        elif formatstyle == "MIN":
+            pass
+        elif formatstyle == "COMPATIBLE":
+            print("Runtime.begin", i)
+
+        run_plugins = [get_plugin(p) for p in plugins if p not in CLI_PLUGINS and
+                       type(get_plugin(p)) not in basic_dt]
+
+        if "lex" in plugins:
+            run_program = lex(run, i, debug=verbose_lvl >= 2,
+                              enable_colors=nocolors == False, tracking=verbose_lvl >= 2)
+            return True
+
+        if "parse" in plugins:
+            run_program = parse(run, i, parser_kwargs={
+                "tracking": verbose_lvl >= 2,
+                "enable_colors": nocolors == False,
+                "debug": verbose_lvl >= 2,
+            }, debug=verbose_lvl >= 3)
+            if verbose_lvl >= 2:
+                if not benchmarking_mods["enabled"]:
+                    if formatstyle == "COMPATIBLE":
+                        print("Program.begin", i)
+                    printers.nprint(run_program, max_level=0, pallete=None if nocolors else COLORS,
+                                    noglyph=noglyph, program_name=i, evaluate=False)
+                    if formatstyle == "COMPATIBLE":
+                        print("Program.end")
+
+                else:
+                    if "benchmarking_parse" not in shown_msgs.keys():
+                        count = str(len(run.splitlines()))
+                        shown_msgs["benchmarking_parse"] = True
+                        if formatstyle == "DEFAULT":
+                            print(colors["2"] + "       - " + colors["H"] +
+                                  count + " line(s) of code Total." + colors["R"])
+                        elif formatstyle == "COMPATIBLE":
+                            print("Benchmark.info:", count)
+
+        run_program = interpret(run, i,
+                                plugins=run_plugins,
+                                debug=verbose_lvl >= 3, enable_colors=nocolors == False,
+                                parser_kwargs={
+                                    "tracking": verbose_lvl >= 2,
+                                    "enable_colors": True,
+                                    "debug": verbose_lvl >= 3,
+                                }
+                                )
+        if verbose_lvl >= 2:
+            if not benchmarking_mods["enabled"]:
+                if formatstyle == "COMPATIBLE":
+                    print("Program.begin", i)
+                printers.nprint(run_program, max_level=0, pallete=None if nocolors else COLORS,
+                                noglyph=noglyph, program_name=i, evaluate=True)
+                if formatstyle == "COMPATIBLE":
+                    print("Program.end")
+            else:
+                if "benchmarking_parse" not in shown_msgs.keys():
+                    count = str(len(run.splitlines()))
+                    shown_msgs["benchmarking_parse"] = True
+                    if formatstyle == "DEFAULT":
+                        print(colors["2"] + "       - " + colors["H"] +
+                              count + " line(s) of code Total." + colors["R"])
+                    elif formatstyle == "COMPATIBLE":
+                        print("Benchmark.info.loc_count", count)
+
+                if "benchmarking_intr" not in shown_msgs.keys():
+                    count = str(len(run_program.flat_blocks))
+                    shown_msgs["benchmarking_intr"] = True
+                    if formatstyle == "DEFAULT":
+                        print(colors["2"] + "       - " + colors["H"] +
+                              count + " blocks(s) Total." + colors["R"])
+                    elif formatstyle == "COMPATIBLE":
+                        print("Benchmark.info.block_count", count)
+
+        if "benchmarking_parse" in shown_msgs.keys():
+            del shown_msgs["benchmarking_parse"]
+        if "benchmarking_intr" in shown_msgs.keys():
+            del shown_msgs["benchmarking_intr"]
+
+        if run_program == None:
+            print("None")
+        if "json" in plugins:
+            if formatstyle == "COMPATIBLE":
+                print("Plugin.json.begin")
+            print(json.dumps(run_program.json, indent=4))
+            if formatstyle == "COMPATIBLE":
+                print("Plugin.json.end")
+
+        if "view" in plugins:
+            if run_program:
+                if not hasattr(run_program, "dot_source"):
+                    if formatstyle == "DEFAULT":
+                        print(
+                            colors["E"] + 'Error: Program does not have dot_source.' + colors["R"], file=sys.stderr)
+                    elif formatstyle == "COMPATIBLE":
+                        print("Plugin.view.error",
+                              "Program does not have dot_source.")
+                    exit(1)
+
+                if formatstyle == "DEFAULT":
+                    graph = GraphvizSource(
+                        run_program.dot_source, filename=tmpdir + "/" + i + ".dot", format="png")
+                    graph.view()
+                elif formatstyle == "COMPATIBLE":
+                    print("Plugin.dot.begin")
+                    print(run_program.dot_source)
+                    print("Plugin.dot.end")
+            else:
+                if formatstyle == "DEFAULT":
+                    print("Nothing to view")
+                elif formatstyle == "COMPATIBLE":
+                    print("Plugin.view.info", "Nothing to view")
+
+    sys.exit(0)
+
+
+def caller(the_call, _type="subprocess", shell=True, ret=False, stdout=-1, stderr=-1):
+    """Calls a shell command, or a program."""
+
+    if _type == "os":
+        proc = subprocess.Popen(the_call,
+                                shell=shell,
+                                stdout=stdout,
+                                bufsize=-1,
+                                stderr=stderr,
+                                # preexec_fn=os.setsid
+                                )
+        if ret:
+            return proc
+        try:
+            p = os._wrap_close(io.TextIOWrapper(proc.stdout), proc)
+            return p.read()
+        except KeyboardInterrupt:
+            os.killpg(os.getpgid(proc.pid), signal.SIGTERM)
+            return False
+
+    elif _type == "subprocess":
+        p = subprocess.Popen(the_call, shell=shell,
+                             stderr=stderr, stdout=stdout)
+        return p
+
+
+def BENCHMARK(input_file, kwargs={}):
+    import math
+
+    if kwargs:
+        quiet = kwargs["quiet"]
+        verbose = kwargs["verbose"]
+        verbose_lvl = kwargs["verbose_lvl"]
+        demos = kwargs["demos"]
+        plugins = kwargs["plugins"]
+        nocolors = kwargs["nocolors"]
+        noglyph = kwargs["noglyph"]
+        formatstyle = kwargs["formatstyle"]
+        benchmarking = kwargs["benchmarking"]
+        benchmarking_mods = kwargs["benchmarking_mods"]
+        colors = kwargs["colors"]
+
+    shown_msgs = {}
+    py = "python"
+    if formatstyle == "DEFAULT":
+        printers.cprint(colors["2"] + "--" + colors["2"] + "== " + colors["2"] +
+                        "Benchmarking..." + colors["2"] + " ==" + colors["2"] + "--" + colors["R"], color="" if nocolors else "SUCCESS")
+    elif formatstyle == "COMPATIBLE":
+        print("Benchmark.begin")
+
+    sys_argv_ = sys.argv
+    sys_argv_.pop(0)
+    sys_argv_.append("--benchmark-mods")
+    sys_argv_.append(
+        "lengthofcode=" + str(benchmarking[1]) + "," +
+        "iterations=" + str(benchmarking[0]) + ""
+    )
+
+    iterations = 0
+    err_count = 0
+    timelog = []
+
+    while iterations < int(benchmarking[0]):
+        # Open a subprocess for running the wanted command...
+        try:
+            # Remove the benchmark arguments and pass the rest to the caller.
+            strings = sys_argv_
+            for string in strings:
+                if string == "-b" or string == "--benchmark":
+                    pos = strings.index(string) + 1
+                    if benchmarking[0] != 0:
+                        if benchmarking[0] == strings[pos]:
+                            strings.pop(pos)
+                            pos -= 1
+                    if benchmarking[1] != 0:
+                        if benchmarking[1] == strings[pos + 1]:
+                            strings.pop(pos + 1)
+                            pos -= 1
+                    strings.remove(string)
+                    break
+
+            p = caller([sys.executable, __file__] + strings, _type="subprocess", shell=False, ret=True)
+            pout = os._wrap_close(io.TextIOWrapper(p.stdout), p)
+            perr = os._wrap_close(io.TextIOWrapper(p.stderr), p)
+
+            t_start = perf_counter()
+            read_total_perr = ""
+            read_total_pout = ""
+            for c in itertools.cycle([
+                '⡀', '⠄', '⠂', '⠁', '⠈', '⠐', '⠠', '⢀',
+            ]):
+                if "benchmark_first_iteration" not in shown_msgs.keys():
+                    read_pout = pout.read()
+                    read_perr = perr.read()
+                    read_total_pout = read_total_pout + "\n" + read_pout
+                    read_total_perr = read_total_perr + "\n" + read_perr
+                    if read_pout != "":
+                        if formatstyle == "DEFAULT":
+                            print(colors["2"] + "       OUT: " +
+                                  colors["R"] + read_pout)
+                        elif formatstyle == "COMPATIBLE":
+                            print("Benchmark.out", read_pout)
+                    if read_perr != "":
+                        if formatstyle == "DEFAULT":
+                            print(colors["E"] + "       ERR: " +
+                                  colors["R"] + read_perr)
+                        elif formatstyle == "COMPATIBLE":
+                            print("Benchmark.err", read_perr)
+                        raise TimeoutError("An error occured, aborting..")
+                if p.poll() != None:
+                    shown_msgs["benchmark_first_iteration"] = True
+                    break
+                else:
+                    if formatstyle == "DEFAULT":
+                        sys.stdout.write('\r' + c + ' ' +
+                                         "inst: " + str(iterations) + "  ")
+                        sys.stdout.flush()
+                    sleep(0.033)
+            t_end = perf_counter()
+        except KeyboardInterrupt:
+            if formatstyle == "DEFAULT":
+                print(colors["GREEN"] +
+                      "\nUser cancelled (KeyboardInterrupt)" + colors["R"])
+                printers.cprint(colors["2"] + "--" + colors["2"] + "== " + colors["2"] +
+                                "Benchmarking done..." + colors["2"] + " ==" + colors["2"] + "--" + colors["R"] + "\n", color="" if nocolors else "SUCCESS")
+            elif formatstyle == "COMPATIBLE":
+                print("Benchmark.cancelled")
+                print("Benchmark.end")
+
+            exit(0)
+        except TimeoutError as e:
+            if formatstyle == "DEFAULT":
+                print(colors["GREEN"] + "Timeout: " + str(e) + colors["R"])
+                printers.cprint(colors["2"] + "--" + colors["2"] + "== " + colors["2"] +
+                                "Benchmarking done..." + colors["2"] + " ==" + colors["2"] + "--" + colors["R"] + "\n", color="" if nocolors else "SUCCESS")
+            elif formatstyle == "COMPATIBLE":
+                print("Benchmark.timeout", str(e))
+                print("Benchmark.end")
+            exit(1)
+
+        timelog.append({
+            "iteration": iterations,
+            "start": t_start,
+            "end": t_end,
+            "stdout": read_total_pout,
+            "stderr": read_total_perr,
+        })
+
+        iterations += 1
+
+    if formatstyle == "DEFAULT":
+        sys.stdout.write('\r' + 'Total iterations: ' + str(iterations) + '\n')
+    elif formatstyle == "COMPATIBLE":
+        sys.stdout.write('Benchmark.info.total_iter ' + str(iterations) + '\n')
+    sys.stdout.flush()
+
+    if formatstyle == "DEFAULT":
+        [print(str(t["iteration"]) + " => " + str(round((t["end"] - t["start"]) *
+                                                        1000, 1000))[:6] + " ms") for t in timelog]
+    elif formatstyle == "COMPATIBLE":
+        [print("Benchmark.info.iter", str(t["iteration"]) + " " + str(round((t["end"] - t["start"]) *
+                                                                            1000, 1000))[:6] + " ms") for t in timelog]
+
+    durations = [t["end"] - t["start"] for t in timelog]
+    if formatstyle == "DEFAULT":
+        print(colors["1"] + "Max: " + colors["HEADER"] + str(round((max(durations)) *
+                                                                   1000, 1000))[:6] + colors["1"] + " ms" + colors["R"])
+        print(colors["1"] + "Min: " + colors["HEADER"] + str(round((min(durations)) *
+                                                                   1000, 1000))[:6] + colors["1"] + " ms" + colors["R"])
+        print(colors["1"] + "Avg: " + colors["HEADER"] + str(round((sum(durations) /
+                                                                    iterations) * 1000, 1000))[:6] + colors["1"] + " ms" + colors["R"])
+        printers.cprint(colors["2"] + "--" + colors["2"] + "== " + colors["2"] +
+                        "Benchmarking done..." + colors["2"] + " ==" + colors["2"] + "--" + colors["R"] + "\n", color="" if nocolors else "SUCCESS")
+    elif formatstyle == "COMPATIBLE":
+        print("Benchmark.info.max", str(round((max(durations)) *
+                                              1000, 1000))[:6])
+        print("Benchmark.info.min", str(round((min(durations)) *
+                                              1000, 1000))[:6])
+        print("Benchmark.info.avg", str(round((sum(durations) /
+                                               iterations) * 1000, 1000))[:6])
+        print("Benchmark.end")
+
+    exit(0)
+
+
+def main():
+    e3lm_parser = argparse.ArgumentParser(prog='e3lm',
+                                          usage='%(prog)s [options] file',
+                                          description=__doc__,
+                                          formatter_class=argparse.RawTextHelpFormatter,
+                                          epilog=__doc2__)
+
+    e3lm_parser.add_argument('--version', action="version",
+                             version="e3lm CLI v" + __version__ + " (3lm language)")
+
+    e3lm_parser.add_argument('file',
+                             nargs='?',
+                             default='-',
+                             help='path to the 3lm file (automatically detects extension) or - for nothing',
+                             )
+
+    e3lm_parser.add_argument('-q',
+                             '--quiet',
+                             action='store_true',
+                             dest='quiet',
+                             default=False,
+                             help='run quietly without any output')
+
+    e3lm_parser.add_argument('-nc',
+                             '--no-color',
+                             action='store_true',
+                             dest="nocolors",
+                             default=False,
+                             help='set output to be without ANSI colors')
+
+    e3lm_parser.add_argument('-ng',
+                             '--no-glyph',
+                             action='store_true',
+                             dest="noglyph",
+                             default=False,
+                             help='use non-glyph character to avoid encoding issues')
+
+    e3lm_parser.add_argument('-v',
+                             '--verbose',
+                             action='store',
+                             metavar='NONE|ERROR|INFO|DEBUG',
+                             dest='verbose',
+                             type=str,
+                             choices=["NONE", "ERROR", "INFO", "DEBUG"],
+                             default="INFO",
+                             help='filter output messages (default is INFO)')
+
+    # e3lm_parser.add_argument('-i',
+    #                          '--interactive',
+    #                          action='store_true',
+    #                          default=False,
+    #                          help='execute with interactive mode')
+
+    e3lm_parser.add_argument('-p',
+                             '--plugin',
+                             action='store',
+                             metavar='plugin',
+                             type=str,
+                             default="",
+                             nargs="+",
+                             help='interpret using plugin(s). see below')
+
+    e3lm_parser.add_argument('-d',
+                             '--demo',
+                             dest='demo',
+                             metavar="code<n>",
+                             action='store',
+                             nargs='+',
+                             type=str,
+                             help='interpret demos in addition'
+                             )
+
+    e3lm_parser.add_argument('-b',
+                             '--benchmark',
+                             metavar='N',
+                             dest='benchmarking',
+                             default=False,
+                             action=arg_required_length(0, 2),
+                             nargs="*",
+                             help="Benchmark N number of times [and N times length of code]",
+                             )
+
+    e3lm_parser.add_argument('-fs',
+                             '--formatstyle',
+                             action='store',
+                             metavar='DEFAULT|MIN|COMPATIBLE',
+                             dest='formatstyle',
+                             type=str,
+                             choices=["DEFAULT", "MIN", "COMPATIBLE"],
+                             default="DEFAULT",
+                             help='Formatting of the output messages',
+                             )
+
+    # For passing BENCHMARK to subprocess to modify length of codes.
+    e3lm_parser.add_argument('--benchmark-mods',
+                             dest='benchmarking_mods',
+                             required=False, type=str,
+                             help=argparse.SUPPRESS)
+
+    args = e3lm_parser.parse_args()
+
+    quiet = args.quiet
+    if quiet:
+        verbose = "NONE"
+    verbose = args.verbose.upper()
+    verbose_lvl = 1 if verbose == "ERROR" else 2 if verbose == "INFO" else 3 if verbose == "DEBUG" else 0
+    input_file = args.file
+    demos = args.demo or []
+    plugins = args.plugin or []
+    nocolors = args.nocolors
+    noglyph = args.noglyph
+    formatstyle = args.formatstyle
+
+    colors = COLORS
+    if nocolors:
+        colors = {k: "" for k in COLORS.keys()}
+    benchmarking = args.benchmarking
+    benchmarking_mods = args.benchmarking_mods
+    if benchmarking_mods == None:
+        benchmarking_mods = {}
+        benchmarking_mods["enabled"] = False
+    else:
+        benchmarking_mods = benchmarking_mods.split(",")
+        benchmarking_mods = {b.split('=')[0]: b.split(
+            '=')[1] for b in benchmarking_mods}
+        benchmarking_mods["enabled"] = True
+
+    kwargs = {
+        "args": args,
+        "quiet": quiet,
+        "verbose": verbose,
+        "verbose_lvl": verbose_lvl,
+        "demos": demos,
+        "plugins": plugins,
+        "nocolors": nocolors,
+        "noglyph": noglyph,
+        "formatstyle": formatstyle,
+        "benchmarking": benchmarking,
+        "benchmarking_mods": benchmarking_mods,
+        "colors": colors,
+        "e3lm_parser": e3lm_parser,
+    }
+
+    # --- Check if benchmarking ---
+    if benchmarking != False:
+        if type(benchmarking) == list:
+            if len(benchmarking) == 0:
+                benchmarking = [1, 1, ]
+            elif len(benchmarking) == 1:
+                benchmarking.append(1)
+        if benchmarking[0] != 0 and benchmarking[1] != 0:
+            BENCHMARK(input_file, kwargs=kwargs)
+    else:
+        # --- Actual program ---
+        CLI(input_file, kwargs=kwargs)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `e3lm-0.1.8/src/e3lm/contrib/json.py` & `e3lm-0.1.9/src/e3lm/contrib/json.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-"""
-Author: Kenan Masri
-
-`JsonPlugin` is an E3lm interpreter plugin used to provide a `json` attribute
-to the main program, containing a json string.
-The plugin can have options such as `ast` to determine whether to generate
-an AST or a tree with evaluated attributes.
-"""
-import json
-from e3lm.helpers.printers import cprint
-from e3lm.lang.interpreters import E3lmInterpreter
-from e3lm.lang import ast
-
-
-class JsonPlugin(E3lmInterpreter):
-    """An E3lm interpreter plugin used to provide a `json` attribute to the
-    main program, containing a json string."""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.options = kwargs
-
-    def interpret(self, input, source=None):
-        self.program = input
-        program_json = self.visit(self.program)
-        self.program.json = program_json
-        return self.program
-
-    def v_Program(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        s = {**s,
-             "imports": obj.imports,
-             }
-        s["blocks"] = []
-        for i, b in enumerate(obj.blocks):
-            s["blocks"].append(self.visit(b))
-        return s
-
-    def v_Block(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        s = {**s,
-             "name": obj.name,
-             "type": obj.type,
-             }
-        s["attrs"] = {}  # Attrs first in s then children.
-        s["children"] = []
-
-        # Visit children first then attributes.
-        for i, b in enumerate(obj.children):
-            s["children"].append(self.visit(b))
-
-        # Get the ast option. If not specified, detect from post or pre plugin.
-        self.from_ast = self.options["ast"] \
-            if "ast" in self.options.keys() else None
-        if self.from_ast == None:
-            self.from_ast = False
-            if hasattr(self, "is_plugin") and self.is_plugin == True:
-                if self.is_pre:
-                    from_ast = True
-            elif hasattr(self, "is_pre") and self.is_pre == True:
-                from_ast = True
-        if self.from_ast:
-            # Get the ast attribute values.
-            for i, a in obj._attrs.items():
-                s["attrs"][i] = self.visit(a)
-        else:
-            # Get the visited attribute values.
-            for i, a in obj.attrs.items():
-                s["attrs"][i] = self.visit(a)
-        return s
-
-    def vgeneric_start(self, obj, *args, **kwargs):
-        s = {
-            "_type": obj.__class__.__name__,
-        }
-        return s
-
-    def vgeneric_value(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        s["value"] = self.visit(obj.value)
-        return s
-
-    def vgeneric_children(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        s["children"] = [self.visit(a) for a in obj.children]
-        return s
-
-    def vgeneric_string(self, obj, *args, **kwargs):
-        s = str(obj)
-        return s
-
-    def v_Func(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        s["value"] = obj.value
-        s["children"] = []
-        if obj.children:
-            s["children"] = [self.visit(a) for a in obj.children]
-        return s
-
-    def v_Num(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        # Stringify the values not supported by JSON
-        s["type"] = obj.type
-        s["value"] = obj.eval if s["type"] in ("NUM_INT", "NUM_FLOAT",) \
-            else str(obj.value)
-        return s
-
-    def v_Str(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        s["type"] = obj.type
-        s["value"] = obj.value
-        return s
-
-    def v_Undefined(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        s["value"] = "null"
-        return s
-
-    # Visiting OPs is implied when ast option is True.
-    def v_BinOp(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        s["op"] = obj.op
-        s["right"] = self.visit(obj.right)
-        s["left"] = self.visit(obj.left)
-        return s
-
-    def v_UnaryOp(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        s["op"] = obj.op
-        s["value"] = self.visit(obj.value)
-        return s
-
-    def v_DictCouple(self, obj, *args, **kwargs):
-        s = self.vgeneric_start(obj)
-        s["left"] = self.visit(obj.left)
-        s["right"] = self.visit(obj.right)
-        return s
-
-    def v_Attr(self, obj, *args, **kwargs):
-        # Names are the keys of the dict "attrs" of block.
-        s = self.vgeneric_start(obj)
-        s["value"] = self.visit(obj.value)
-        if hasattr(obj, "tokens"):
-            s["tokens"] = obj.tokens
-        return s
-
-    v_Type = vgeneric_value
-    v_Identifier = vgeneric_children
-    v_Index = vgeneric_value
-    v_Array = vgeneric_children
-    v_Dict = vgeneric_children
-    v_Bool = vgeneric_value
-
-    def v_dict(self, obj, *args, **kwargs):
-        d = {}
-        for i, j in obj.items():
-            if type(i) not in (str, int,):  # Dict keys must be int or str.
-                if type(i) == ast.Identifier:
-                    i = i.children[0]
-                if type(i) == ast.Num \
-                        or type(i) == ast.Str:
-                    i = self.visit(i)["value"]
-            d[i] = self.visit(j)
-        return d
-
-    def v_list(self, obj, *args, **kwargs):
-        l = []
-        for i, j in enumerate(obj):
-            l.append(self.visit(j))
-        return l
-
-    def v_bool(self, obj, *args, **kwargs):
-        return obj
-
-    v_tuple = vgeneric_string
-    v_complex = vgeneric_string
+"""
+Author: Kenan Masri
+
+`JsonPlugin` is an E3lm interpreter plugin used to provide a `json` attribute
+to the main program, containing a json string.
+The plugin can have options such as `ast` to determine whether to generate
+an AST or a tree with evaluated attributes.
+"""
+import json
+from e3lm.helpers.printers import cprint
+from e3lm.lang.interpreters import E3lmInterpreter
+from e3lm.lang import ast
+
+
+class JsonPlugin(E3lmInterpreter):
+    """An E3lm interpreter plugin used to provide a `json` attribute to the
+    main program, containing a json string."""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.options = kwargs
+
+    def interpret(self, input, source=None):
+        self.program = input
+        program_json = self.visit(self.program)
+        self.program.json = program_json
+        return self.program
+
+    def v_Program(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        s = {**s,
+             "imports": obj.imports,
+             }
+        s["blocks"] = []
+        for i, b in enumerate(obj.blocks):
+            s["blocks"].append(self.visit(b))
+        return s
+
+    def v_Block(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        s = {**s,
+             "name": obj.name,
+             "type": obj.type,
+             }
+        s["attrs"] = {}  # Attrs first in s then children.
+        s["children"] = []
+
+        # Visit children first then attributes.
+        for i, b in enumerate(obj.children):
+            s["children"].append(self.visit(b))
+
+        # Get the ast option. If not specified, detect from post or pre plugin.
+        self.from_ast = self.options["ast"] \
+            if "ast" in self.options.keys() else None
+        if self.from_ast == None:
+            self.from_ast = False
+            if hasattr(self, "is_plugin") and self.is_plugin == True:
+                if self.is_pre:
+                    from_ast = True
+            elif hasattr(self, "is_pre") and self.is_pre == True:
+                from_ast = True
+        if self.from_ast:
+            # Get the ast attribute values.
+            for i, a in obj._attrs.items():
+                s["attrs"][i] = self.visit(a)
+        else:
+            # Get the visited attribute values.
+            for i, a in obj.attrs.items():
+                s["attrs"][i] = self.visit(a)
+        return s
+
+    def vgeneric_start(self, obj, *args, **kwargs):
+        s = {
+            "_type": obj.__class__.__name__,
+        }
+        return s
+
+    def vgeneric_value(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        s["value"] = self.visit(obj.value)
+        return s
+
+    def vgeneric_children(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        s["children"] = [self.visit(a) for a in obj.children]
+        return s
+
+    def vgeneric_string(self, obj, *args, **kwargs):
+        s = str(obj)
+        return s
+
+    def v_Func(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        s["value"] = obj.value
+        s["children"] = []
+        if obj.children:
+            s["children"] = [self.visit(a) for a in obj.children]
+        return s
+
+    def v_Num(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        # Stringify the values not supported by JSON
+        s["type"] = obj.type
+        s["value"] = obj.eval if s["type"] in ("NUM_INT", "NUM_FLOAT",) \
+            else str(obj.value)
+        return s
+
+    def v_Str(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        s["type"] = obj.type
+        s["value"] = obj.value
+        return s
+
+    def v_Undefined(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        s["value"] = "null"
+        return s
+
+    # Visiting OPs is implied when ast option is True.
+    def v_BinOp(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        s["op"] = obj.op
+        s["right"] = self.visit(obj.right)
+        s["left"] = self.visit(obj.left)
+        return s
+
+    def v_UnaryOp(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        s["op"] = obj.op
+        s["value"] = self.visit(obj.value)
+        return s
+
+    def v_DictCouple(self, obj, *args, **kwargs):
+        s = self.vgeneric_start(obj)
+        s["left"] = self.visit(obj.left)
+        s["right"] = self.visit(obj.right)
+        return s
+
+    def v_Attr(self, obj, *args, **kwargs):
+        # Names are the keys of the dict "attrs" of block.
+        s = self.vgeneric_start(obj)
+        s["value"] = self.visit(obj.value)
+        if hasattr(obj, "tokens"):
+            s["tokens"] = obj.tokens
+        return s
+
+    v_Type = vgeneric_value
+    v_Identifier = vgeneric_children
+    v_Index = vgeneric_value
+    v_Array = vgeneric_children
+    v_Dict = vgeneric_children
+    v_Bool = vgeneric_value
+
+    def v_dict(self, obj, *args, **kwargs):
+        d = {}
+        for i, j in obj.items():
+            if type(i) not in (str, int,):  # Dict keys must be int or str.
+                if type(i) == ast.Identifier:
+                    i = i.children[0]
+                if type(i) == ast.Num \
+                        or type(i) == ast.Str:
+                    i = self.visit(i)["value"]
+            d[i] = self.visit(j)
+        return d
+
+    def v_list(self, obj, *args, **kwargs):
+        l = []
+        for i, j in enumerate(obj):
+            l.append(self.visit(j))
+        return l
+
+    def v_bool(self, obj, *args, **kwargs):
+        return obj
+
+    v_tuple = vgeneric_string
+    v_complex = vgeneric_string
```

### Comparing `e3lm-0.1.8/src/e3lm/contrib/units.py` & `e3lm-0.1.9/src/e3lm/contrib/units.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-"""
-Author: Kenan Masri
-
-`UnitsPlugin` is an E3lm interpreter plugin used to pick Attrs that end with
-"_unit", create a `Unit` object and relate it to the main attribute without the
-ending.
-
-Eventually matching Attrs will have a `Unit` attached thereto.
-"""
-import sys
-from copy import deepcopy
-from e3lm.helpers.printers import cprint
-from e3lm.lang.interpreters import E3lmPlugin
-from e3lm.lang import ast
-
-
-class Unit():
-    """Base unit."""
-
-    def __init__(self, id="unit", name="units", **kwargs):
-        self.id = id
-        self.name = name
-        self.converts_to = {}
-        if "converts_to" in kwargs.keys():
-            self.converts_to = kwargs["converts_to"]
-        if type(self.converts_to) in (set, list, tuple):
-            sett = self.converts_to
-            self.converts_to = {}
-
-            for s in sett[1].converts_to:
-                val = sett[1].converts_to[s]
-                self.converts_to[s] = sett[0]*val
-
-    def convert(self, target, amount):
-        if type(target) != Unit:
-            for ustr in [g for g in dir(sys.modules[__name__])
-                         if not g.startswith('_')]:
-                u = getattr(sys.modules[__name__], ustr)
-                if type(u) == Unit:
-                    if u.id == target:
-                        target = u
-        if type(target) == Unit:
-            return amount * self.converts_to[target.id]
-        else:
-            raise ValueError("Cannot convert from {} to {}".format(
-                self.id, target))
-
-    def __str__(self):
-        return "Unit("+self.id+")"
-
-
-inch = Unit("in", "inches", converts_to={
-    "px": 96,
-    "pt": 72,
-    "pc": 6,
-    "cm": 2.54,
-    "mm": 25.4,
-    "m": 0.0254,
-    "in": 1.0,
-})
-cm = Unit("cm", "centimeters", converts_to={
-    "px": 37.79527559055118,
-    "pt": 28.346456692913385,
-    "pc": 2.3622047244094486,
-    "mm": 10.0,
-    "cm": 1.0,
-    "m": 0.01,
-    "in": 0.39370078740157477,
-})
-mm = Unit("mm", "millimeters", converts_to=(0.1, cm))
-m = Unit("m", "meters", converts_to=(100, cm))
-km = Unit("km", "kilometers", converts_to=(1000, m))
-px = Unit("px", "pixels", converts_to=(1/96, inch))
-pt = Unit("pt", "points", converts_to=(1/72, inch))
-pc = Unit("pc", "picas", converts_to=(12, pt))
-
-
-class UnitsPlugin(E3lmPlugin):
-    """An E3lm interpreter plugin used to pick Attrs that end with "_unit",
-    create a `Unit` object and relate it to the main attribute without the
-    ending."""
-
-    def __init__(self, *args, **kwargs):
-        self.options = kwargs
-        self.units = {
-            "inch": inch,
-            "cm": cm,
-            "mm": mm,
-            "m": m,
-            "km": km,
-            "px": px,
-            "pt": pt,
-            "pc": pc,
-        }
-
-    def interpret(self, input, source=None):
-        return self.visit(input)
-
-    def v_Program(self, obj, *args, **kwargs):
-        for i, b in enumerate(obj.blocks):
-            obj.blocks[i] = b = self.visit(b)
-        return obj
-
-    def v_Block(self, obj, *args, **kwargs):
-        for i, b in enumerate(obj.children):
-            obj.children[i] = b = self.visit(b)
-
-        nattrs = [a.name for i, a in obj._attrs.items()]
-        vattrs = []
-        for i, a in obj._attrs.items():
-            if a.name.endswith("_unit"):
-                if a.name[:-5] in nattrs:
-                    vattrs.append((a, a.name[:-5]))
-
-        for s in vattrs:
-            obj._attrs[s[0]] = self.v_Attr(s[0], obj._attrs[s[1]])
-        return obj
-
-    def v_Attr(self, obj, main_attr):
-        main_attr.unit = deepcopy(self.units[obj.eval])
-        main_attr.convert = lambda u: main_attr.unit.convert(u, main_attr.eval)
-        return obj
+"""
+Author: Kenan Masri
+
+`UnitsPlugin` is an E3lm interpreter plugin used to pick Attrs that end with
+"_unit", create a `Unit` object and relate it to the main attribute without the
+ending.
+
+Eventually matching Attrs will have a `Unit` attached thereto.
+"""
+import sys
+from copy import deepcopy
+from e3lm.helpers.printers import cprint
+from e3lm.lang.interpreters import E3lmPlugin
+from e3lm.lang import ast
+
+
+class Unit():
+    """Base unit."""
+
+    def __init__(self, id="unit", name="units", **kwargs):
+        self.id = id
+        self.name = name
+        self.converts_to = {}
+        if "converts_to" in kwargs.keys():
+            self.converts_to = kwargs["converts_to"]
+        if type(self.converts_to) in (set, list, tuple):
+            sett = self.converts_to
+            self.converts_to = {}
+
+            for s in sett[1].converts_to:
+                val = sett[1].converts_to[s]
+                self.converts_to[s] = sett[0]*val
+
+    def convert(self, target, amount):
+        if type(target) != Unit:
+            for ustr in [g for g in dir(sys.modules[__name__])
+                         if not g.startswith('_')]:
+                u = getattr(sys.modules[__name__], ustr)
+                if type(u) == Unit:
+                    if u.id == target:
+                        target = u
+        if type(target) == Unit:
+            return amount * self.converts_to[target.id]
+        else:
+            raise ValueError("Cannot convert from {} to {}".format(
+                self.id, target))
+
+    def __str__(self):
+        return "Unit("+self.id+")"
+
+
+inch = Unit("in", "inches", converts_to={
+    "px": 96,
+    "pt": 72,
+    "pc": 6,
+    "cm": 2.54,
+    "mm": 25.4,
+    "m": 0.0254,
+    "in": 1.0,
+})
+cm = Unit("cm", "centimeters", converts_to={
+    "px": 37.79527559055118,
+    "pt": 28.346456692913385,
+    "pc": 2.3622047244094486,
+    "mm": 10.0,
+    "cm": 1.0,
+    "m": 0.01,
+    "in": 0.39370078740157477,
+})
+mm = Unit("mm", "millimeters", converts_to=(0.1, cm))
+m = Unit("m", "meters", converts_to=(100, cm))
+km = Unit("km", "kilometers", converts_to=(1000, m))
+px = Unit("px", "pixels", converts_to=(1/96, inch))
+pt = Unit("pt", "points", converts_to=(1/72, inch))
+pc = Unit("pc", "picas", converts_to=(12, pt))
+
+
+class UnitsPlugin(E3lmPlugin):
+    """An E3lm interpreter plugin used to pick Attrs that end with "_unit",
+    create a `Unit` object and relate it to the main attribute without the
+    ending."""
+
+    def __init__(self, *args, **kwargs):
+        self.options = kwargs
+        self.units = {
+            "inch": inch,
+            "cm": cm,
+            "mm": mm,
+            "m": m,
+            "km": km,
+            "px": px,
+            "pt": pt,
+            "pc": pc,
+        }
+
+    def interpret(self, input, source=None):
+        return self.visit(input)
+
+    def v_Program(self, obj, *args, **kwargs):
+        for i, b in enumerate(obj.blocks):
+            obj.blocks[i] = b = self.visit(b)
+        return obj
+
+    def v_Block(self, obj, *args, **kwargs):
+        for i, b in enumerate(obj.children):
+            obj.children[i] = b = self.visit(b)
+
+        nattrs = [a.name for i, a in obj._attrs.items()]
+        vattrs = []
+        for i, a in obj._attrs.items():
+            if a.name.endswith("_unit"):
+                if a.name[:-5] in nattrs:
+                    vattrs.append((a, a.name[:-5]))
+
+        for s in vattrs:
+            obj._attrs[s[0]] = self.v_Attr(s[0], obj._attrs[s[1]])
+        return obj
+
+    def v_Attr(self, obj, main_attr):
+        main_attr.unit = deepcopy(self.units[obj.eval])
+        main_attr.convert = lambda u: main_attr.unit.convert(u, main_attr.eval)
+        return obj
```

### Comparing `e3lm-0.1.8/src/e3lm/demos/data.py` & `e3lm-0.1.9/src/e3lm/demos/data.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,298 +1,298 @@
-examples = []
-
-
-def getcode(num, prefix="code"):
-    code = globals().get(prefix + str(num), "")
-    if code != "":
-        return code
-    else:
-        return None
-
-
-# 0
-code0 = """\
-; Empty block
-Dummy dummy
-End
-"""
-examples.append({"ind": 0, "text": code0,
-                 "lex": {
-                     "assert": [
-                         ["tokens", ['CLASS', 'END']]
-                     ]},
-                 "raises": [],
-                 })
-# 1
-code1 = """; Nested empty blocks
-Dummy dummy_1
-End
-Dummy dummy_2
-    Dummy dummy_2_1
-        Dummy dummy_2_1_1
-            Dummy dummy_2_1_1_1
-            End
-        End
-    End
-End
-Dummy ;unnamed
-End
-"""
-examples.append({"ind": 1, "text": code1,
-                 "lex": {
-                     "assert": [
-                         ["tokens", ['CLASS', 'END', 'CLASS',
-                                     'CLASS', 'CLASS', 'CLASS',
-                                     'END', 'END', 'END', 'END',
-                                     'CLASS', 'END']],
-                     ]},
-                 "dot": True,
-                 "raises": [],
-                 })
-# 2
-code2 = """Dummy dummy_1
-    Dummy dummy_1_1
-        Dummy dummy_1_1_1
-            ; Basic attributes' expressions
-            attr1 = 0
-            attr2 = 0.0
-            attr3 = 0o0
-            attr4 = 0x0
-            attr5 = 0b0
-            attr6 = 3j
-            attr7 = 5 + 3.14e-10j
-            attr8 = "Q2 String"
-            attr9 = 'Q1 String'
-            attr10 = \"\"\"TQ2 String\"\"\"
-            attr11 = '''TQ1 String'''
-            attr12 = None
-            attr13 = True
-            attr14 = False
-            attr15 = \"\"\"TQ2 w\\ quotes: '" I guess\"\"\"
-        End
-        Dummy dummy_1_1_2
-            ; Arithmetic expressions
-            attr1 = 0+1
-            attr2 = 0.0 + 0.1
-            attr3 = 0o5 + 0o11
-            attr4 = 0x5 + 0x9
-            attr5 = 0b1 + 0b111
-            attr6 = 3j + 15j
-            attr7 = (5 + 3j) + (10 + 2j)
-            attr8 = "Q2" + ' ' + '''TQ1'''
-            attr9 = 5 * 2
-            attr10 = 11 / 10
-            attr11 = 11 // 10
-            attr12 = 5 - 5
-        End
-        Dummy dummy_1_1_3
-            ; Complicated attributes
-            attr1 = prev()
-            attr2 = {
-                1: {2: {"hi": "hello"}}
-            }
-            attr3 = attr2
-            attr4 = next().attr2["two"]
-            attr5 = body
-            attr6 = prev(Dummy).attr1
-            attr7 = Dummy
-            attr8 = (5 - (attr4+5) + 5)
-            attr9 = attr8 + prev().attr7
-            attr10 = - attr8
-            attr11 = dummy_1_1_4
-            attr12 = attr11.attr1
-            attr13 = next(Dummy)
-            attr14 = dummy_1_1_4.attr0
-            ;TODO: interpreter error: attr15 = attr14.attr0
-            ---
-             Bodytext
-            ---
-        End
-        Dummy dummy_1_1_4
-            attr0 = "5"
-            ; Arrays and Dicts
-            attr1 = prev().attr1.attr1
-            attr2 = {
-                "one": attr1,
-                "two": 2
-            }
-            attr3a = [
-                "Hi", "There", {"one": 1},
-            ]
-            attr4 = attr3a[2]["one"]
-        End
-    End
-End
-Object
-End
-"""
-examples.append({"ind": 2, "text": code2,
-                 "lex": True,
-                 "parse": True,
-                 "interpret": {
-                     "assert": [
-                         ["dummy_1_1_3.body", "Bodytext"],
-                         ["dummy_1_1_2.attr1", 1],
-                         ["dummy_1_1_2.attr8", "Q2 TQ1"],
-                     ]},
-                 "json": True,
-                 "raises": [],
-                 })
-# 3
-errorcode0 = """\
-Dummy dummy_1_1
-;comment
-    attr0 = 0
-     attr1 = 1
-   attr2 = 0
-End
-"""
-examples.append({"ind": 0, "text": errorcode0,
-                 "lex": {
-                     "assert": [
-                         ["error", {"class": "IndentationError", "lineno": 4}],
-                     ]},
-                 "raises": ["lex", ],
-                 })
-# 4
-errorcode1 = """\
-Dummy dummy_2_1
-    Dummy
-        Dummy dummy_2_2
-    attr1 = 0
-            attr2 = 0
-        ---
-    what
-       ---
-    End
-        End
-  End
-"""
-examples.append({"ind": 1, "text": errorcode1,
-                 "lex": {
-                     "assert": [
-                         ["error", {"class": "IndentationError", "lineno": 5}],
-                     ]},
-                 "parse": True,
-                 "raises": ["lex", ],
-                 })
-# 5
-errorcode2 = """\
-Dummy dummy_2
-;comment
-;comment
-;comment
-;comment
-     attr = 1
-     attr = 2
-     attr = 2
-    ---
-     what
-    ---
-End
-    End
-End
-"""
-examples.append({"ind": 2, "text": errorcode2,
-                 "lex": {
-                     "assert": [
-                         ["error", {"class": "SyntaxError", "lineno": 13}],
-                     ]},
-                 "parse": {
-                     "assert": [
-                         ["p_error", {"class": "AttributeError", "lineno": 7}],
-                         ["p_error", {"class": "AttributeError", "lineno": 8}],
-                     ]},
-                 "raises": ["lex", "parse", ],
-                 })
-# 6
-code3 = """\
-Dummy dummy_1
-    attr1 = attr2
-    attr2 = 2
-    attr3 = name
-End
-Dummy d
-    attr1 = prev().name
-    attr2 = prev(Dummy)
-    attr3 = prev(Dummy).name
-    attr5 = "word".join(attr4)
-    ---rtl
-    مرحبا
-    بكم
-    في
-    مكتبة
-    كنان
-    ---
-    attr4 = body.split("\\n")
-End
-
-Dummy e232
-    body = "ha"
-End
-
-; comment?
-"""
-examples.append({"ind": 3, "text": code3,
-                 "lex": True,
-                 "raises": [],
-                 })
-# 7
-code4 = """\
-Dummy my1
-    attr2 = {
-        0: {
-            "1": {
-                "2": {
-                    "hi": "hello"
-                }
-            }
-        }
-    }
-    attr1 = attr2[0]["1"]["2"]["hi"]
-
-End
-"""
-examples.append({"ind": 4, "text": code4,
-                 "lex": True,
-                 "raises": [],
-                 })
-# 8
-code5 = """\
-Dummy dummy_1
-    attr1 = 1.0
-    attr2 = 5.0
-    attr1_unit = "cm"
-    attr2_unit = "m"
-End
-"""
-examples.append({"ind": 5, "text": code5,
-                 "interpret": True,
-                 "units": {
-                     "assert": [
-                         ["dummy_1.attr1.unit.id", "cm"]
-                     ]},
-                 "raises": [],
-                 })
-# 9
-errorcode3 = """\
-Dummy dummy_2
-;comment
-;comment
-;comment
-;comment
-     attr = 1
-     attr = 2
-     attr = 2
-    ---
-     what
-    ---
-End
-"""
-examples.append({"ind": 3, "text": errorcode3,
-                 "parse": {
-                     "assert": [
-                         ["p_error", {"class": "AttributeError", "lineno": 7}],
-                         ["p_error", {"class": "AttributeError", "lineno": 8}],
-                     ]},
-                 "raises": ["parse", ],
-                 })
+examples = []
+
+
+def getcode(num, prefix="code"):
+    code = globals().get(prefix + str(num), "")
+    if code != "":
+        return code
+    else:
+        return None
+
+
+# 0
+code0 = """\
+; Empty block
+Dummy dummy
+End
+"""
+examples.append({"ind": 0, "text": code0,
+                 "lex": {
+                     "assert": [
+                         ["tokens", ['CLASS', 'END']]
+                     ]},
+                 "raises": [],
+                 })
+# 1
+code1 = """; Nested empty blocks
+Dummy dummy_1
+End
+Dummy dummy_2
+    Dummy dummy_2_1
+        Dummy dummy_2_1_1
+            Dummy dummy_2_1_1_1
+            End
+        End
+    End
+End
+Dummy ;unnamed
+End
+"""
+examples.append({"ind": 1, "text": code1,
+                 "lex": {
+                     "assert": [
+                         ["tokens", ['CLASS', 'END', 'CLASS',
+                                     'CLASS', 'CLASS', 'CLASS',
+                                     'END', 'END', 'END', 'END',
+                                     'CLASS', 'END']],
+                     ]},
+                 "dot": True,
+                 "raises": [],
+                 })
+# 2
+code2 = """Dummy dummy_1
+    Dummy dummy_1_1
+        Dummy dummy_1_1_1
+            ; Basic attributes' expressions
+            attr1 = 0
+            attr2 = 0.0
+            attr3 = 0o0
+            attr4 = 0x0
+            attr5 = 0b0
+            attr6 = 3j
+            attr7 = 5 + 3.14e-10j
+            attr8 = "Q2 String"
+            attr9 = 'Q1 String'
+            attr10 = \"\"\"TQ2 String\"\"\"
+            attr11 = '''TQ1 String'''
+            attr12 = None
+            attr13 = True
+            attr14 = False
+            attr15 = \"\"\"TQ2 w\\ quotes: '" I guess\"\"\"
+        End
+        Dummy dummy_1_1_2
+            ; Arithmetic expressions
+            attr1 = 0+1
+            attr2 = 0.0 + 0.1
+            attr3 = 0o5 + 0o11
+            attr4 = 0x5 + 0x9
+            attr5 = 0b1 + 0b111
+            attr6 = 3j + 15j
+            attr7 = (5 + 3j) + (10 + 2j)
+            attr8 = "Q2" + ' ' + '''TQ1'''
+            attr9 = 5 * 2
+            attr10 = 11 / 10
+            attr11 = 11 // 10
+            attr12 = 5 - 5
+        End
+        Dummy dummy_1_1_3
+            ; Complicated attributes
+            attr1 = prev()
+            attr2 = {
+                1: {2: {"hi": "hello"}}
+            }
+            attr3 = attr2
+            attr4 = next().attr2["two"]
+            attr5 = body
+            attr6 = prev(Dummy).attr1
+            attr7 = Dummy
+            attr8 = (5 - (attr4+5) + 5)
+            attr9 = attr8 + prev().attr7
+            attr10 = - attr8
+            attr11 = dummy_1_1_4
+            attr12 = attr11.attr1
+            attr13 = next(Dummy)
+            attr14 = dummy_1_1_4.attr0
+            ;TODO: interpreter error: attr15 = attr14.attr0
+            ---
+             Bodytext
+            ---
+        End
+        Dummy dummy_1_1_4
+            attr0 = "5"
+            ; Arrays and Dicts
+            attr1 = prev().attr1.attr1
+            attr2 = {
+                "one": attr1,
+                "two": 2
+            }
+            attr3a = [
+                "Hi", "There", {"one": 1},
+            ]
+            attr4 = attr3a[2]["one"]
+        End
+    End
+End
+Object
+End
+"""
+examples.append({"ind": 2, "text": code2,
+                 "lex": True,
+                 "parse": True,
+                 "interpret": {
+                     "assert": [
+                         ["dummy_1_1_3.body", "Bodytext"],
+                         ["dummy_1_1_2.attr1", 1],
+                         ["dummy_1_1_2.attr8", "Q2 TQ1"],
+                     ]},
+                 "json": True,
+                 "raises": [],
+                 })
+# 3
+errorcode0 = """\
+Dummy dummy_1_1
+;comment
+    attr0 = 0
+     attr1 = 1
+   attr2 = 0
+End
+"""
+examples.append({"ind": 0, "text": errorcode0,
+                 "lex": {
+                     "assert": [
+                         ["error", {"class": "IndentationError", "lineno": 4}],
+                     ]},
+                 "raises": ["lex", ],
+                 })
+# 4
+errorcode1 = """\
+Dummy dummy_2_1
+    Dummy
+        Dummy dummy_2_2
+    attr1 = 0
+            attr2 = 0
+        ---
+    what
+       ---
+    End
+        End
+  End
+"""
+examples.append({"ind": 1, "text": errorcode1,
+                 "lex": {
+                     "assert": [
+                         ["error", {"class": "IndentationError", "lineno": 5}],
+                     ]},
+                 "parse": True,
+                 "raises": ["lex", ],
+                 })
+# 5
+errorcode2 = """\
+Dummy dummy_2
+;comment
+;comment
+;comment
+;comment
+     attr = 1
+     attr = 2
+     attr = 2
+    ---
+     what
+    ---
+End
+    End
+End
+"""
+examples.append({"ind": 2, "text": errorcode2,
+                 "lex": {
+                     "assert": [
+                         ["error", {"class": "SyntaxError", "lineno": 13}],
+                     ]},
+                 "parse": {
+                     "assert": [
+                         ["p_error", {"class": "AttributeError", "lineno": 7}],
+                         ["p_error", {"class": "AttributeError", "lineno": 8}],
+                     ]},
+                 "raises": ["lex", "parse", ],
+                 })
+# 6
+code3 = """\
+Dummy dummy_1
+    attr1 = attr2
+    attr2 = 2
+    attr3 = name
+End
+Dummy d
+    attr1 = prev().name
+    attr2 = prev(Dummy)
+    attr3 = prev(Dummy).name
+    attr5 = "word".join(attr4)
+    ---rtl
+    مرحبا
+    بكم
+    في
+    مكتبة
+    كنان
+    ---
+    attr4 = body.split("\\n")
+End
+
+Dummy e232
+    body = "ha"
+End
+
+; comment?
+"""
+examples.append({"ind": 3, "text": code3,
+                 "lex": True,
+                 "raises": [],
+                 })
+# 7
+code4 = """\
+Dummy my1
+    attr2 = {
+        0: {
+            "1": {
+                "2": {
+                    "hi": "hello"
+                }
+            }
+        }
+    }
+    attr1 = attr2[0]["1"]["2"]["hi"]
+
+End
+"""
+examples.append({"ind": 4, "text": code4,
+                 "lex": True,
+                 "raises": [],
+                 })
+# 8
+code5 = """\
+Dummy dummy_1
+    attr1 = 1.0
+    attr2 = 5.0
+    attr1_unit = "cm"
+    attr2_unit = "m"
+End
+"""
+examples.append({"ind": 5, "text": code5,
+                 "interpret": True,
+                 "units": {
+                     "assert": [
+                         ["dummy_1.attr1.unit.id", "cm"]
+                     ]},
+                 "raises": [],
+                 })
+# 9
+errorcode3 = """\
+Dummy dummy_2
+;comment
+;comment
+;comment
+;comment
+     attr = 1
+     attr = 2
+     attr = 2
+    ---
+     what
+    ---
+End
+"""
+examples.append({"ind": 3, "text": errorcode3,
+                 "parse": {
+                     "assert": [
+                         ["p_error", {"class": "AttributeError", "lineno": 7}],
+                         ["p_error", {"class": "AttributeError", "lineno": 8}],
+                     ]},
+                 "raises": ["parse", ],
+                 })
```

### Comparing `e3lm-0.1.8/src/e3lm/helpers/printers.py` & `e3lm-0.1.9/src/e3lm/helpers/printers.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,314 +1,314 @@
-# -*- coding: utf-8 -*-
-
-from asciitree import LeftAligned, Traversal, KeyArgsConstructor
-from asciitree.drawing import BoxStyle
-
-COLORS = {
-    # Default...
-    "NONE": u"",
-    "HEADER": u'\x1b[95m',
-    "INFO": u'\x1b[38;5;164m',
-    "INFO2": u'\x1b[38;5;172m',
-    "SUCCESS": u'\x1b[38;5;173m',
-    "WARNING": u'\x1b[93m',
-    "BLACK": u'\x1b[30m',
-    "RED": u'\x1b[31m',
-    "GREEN": u'\x1b[32m',
-    "GREEN": u'\x1b[32m',
-    "YELLOW": u'\x1b[33m',
-    "BLUE": u'\x1b[34m',
-    "MAGENTA": u'\x1b[35m',
-    "CYAN": u'\x1b[36m',
-    "WHITE": u'\x1b[37m',
-    "DEFAULT": u'\x1b[39m',
-    "CYAN": u'\x1b[36m',
-    "BOLD": u'\x1b[1m',
-    "ITALICS": u'\x1b[3m',
-    "UNDERLINE": u'\x1b[4m',
-    "STRIKE": u'\x1b[9m',
-    "ENDC": u'\x1b[0m',
-    "R": u'\x1b[0m',
-    # From CLI...
-    "H": u'\x1b[95m',  # HEADER
-    "1": u'\x1b[38;5;164m',  # FIRST
-    "2": u'\x1b[38;5;173m',  # SECOND
-    "3": u'\x1b[38;5;177m',  # THIRD
-    "4": u'\x1b[38;5;225m',  # FOURTH
-    "E": u'\x1b[91m',  # ERROR
-    "W": u'\x1b[93m',  # WHITE
-    "R": u'\x1b[0m',  # RESET
-    "B": u'\x1b[1m',  # BOLD
-    "U": u'\x1b[4m',  # UNDERLINE
-
-    "RESET": u'\x1b[0m',
-    "GRAY": u'\x1b[38;5;245m',
-
-    "A": u'\x1b[38;5;164m',  # A
-    "B": u'\x1b[38;5;173m',  # B
-    "C": u'\x1b[38;5;177m',  # C
-    "D": u'\x1b[38;5;225m',  # D
-    "E": u'\x1b[95m',        # E
-    "LOG": u'\x1b[38;5;164m',  # LOGGING TAG
-    "LOG_MSG": u'\x1b[38;5;245m',  # LOGGING MESSAGE
-    "ERROR": u'\x1b[91m',  # ERROR
-}
-
-
-class TraverseArrow(KeyArgsConstructor):
-    pass
-
-
-class TraverseItem(KeyArgsConstructor):
-    pass
-
-
-class TRAVERSE(Traversal):
-    evaluate = False
-    program_name = ""
-
-    def __init__(self, cols=COLORS, charset=[], **kwargs):
-        self.charset = {
-            "Program": chr(4),
-            "Block": "□ ",
-            "TraverseItem": {
-                "Import": " ╰ ",
-                "Attr": "⌐ ",
-                "TraverseArrow": "→",
-                "tokens": "←",
-            },
-        } if charset == [] else charset
-        self.COLS = cols
-        super().__init__(**kwargs) # Pass kwargs to parent
-
-
-    def get_children(self, node):
-        """Return a list of children of a node."""
-        method = 'get_children_of_{}'.format(type(node).__name__)
-        getter = getattr(self, method, None)
-        if getter != None:
-            result = getter(node)
-            return result
-        return []
-
-    # Program node children
-    def get_children_of_Program(self, node):
-        imports = [TraverseItem(type="Import", value=x) for x in node.imports]
-        return [*imports, *node.blocks]
-
-    # Block node children (blocks + attrs + body)
-    def get_children_of_Block(self, block):
-        c = [
-            *block.children,
-            *[TraverseItem(type="Attr", name=a, o=block, value=b, children=self.get_children(b))
-              for a, b in block._attrs.items() if a != "body"],
-        ]
-        if hasattr(block, "body"):
-            c.append(TraverseItem(type="Attr", name="body",
-                     o=block, value=block._attrs["body"]))
-        return c
-
-    # Attr children (as arrows holder)
-    def get_children_of_Attr(self, attr):
-        if self.evaluate:
-            if hasattr(attr, "eval"):
-                return TraverseArrow(left=attr.value, rights=[
-                    f"\"{attr.eval}\"" if type(attr.eval) == str else attr.eval
-                ])
-        return [attr.value]
-
-    # Placeholder
-    def get_children_of_TraverseArrow(self, traverse_arrow):
-        return [*traverse_arrow.rights]
-
-    # Placeholder
-    def get_children_of_TraverseItem(self, traverse_item):
-        return []
-
-    def get_root(self, tree):
-        """Return a node representing the tree root from the tree."""
-        return tree
-
-    def get_text(self, node):
-        """Return the text associated with a node."""
-        method = 'get_text_of_{}'.format(type(node).__name__)
-        getter = getattr(self, method, None)
-        if getter != None:
-            result = getter(node)
-            return result
-        return str(node)
-
-    def get_text_of_Program(self, node):
-        namae = self.COLS["HEADER"] + self.program_name # or node.id
-        return self.COLS["BOLD"] + self.COLS["INFO2"] + " " + self.charset["Program"] + " " + self.COLS["INFO"] + "Program(" + namae + self.COLS["INFO"] + ")" + self.COLS["R"]
-
-    def get_text_of_Block(self, block):
-        idpart = (self.COLS["HEADER"] + self.COLS["UNDERLINE"] +
-                  f"#{block.id}" + self.COLS["R"]) if hasattr(block, "id") else ""
-        namepart = (self.COLS["HEADER"] + ", " + block.name +
-                    self.COLS["R"]) if block.name != "" else ""
-        namae = self.COLS["HEADER"] + block.type + idpart + namepart
-        return self.COLS["INFO2"]+ self.charset["Block"] + self.COLS["INFO"] + "Block(" + namae + self.COLS["INFO"] + ")" + self.COLS["R"]
-
-    def get_text_of_TraverseItem(self, item):
-        if item.type == "Import":
-            return self.COLS["INFO2"] + self.charset["TraverseItem"]["Import"] + self.COLS["GRAY"] + "import " + self.COLS["WHITE"] + item.value + self.COLS["R"]
-        elif item.type == "Attr":
-            attr = item
-            namae = self.COLS["HEADER"] + attr.name + self.COLS["R"]
-            eqq = self.COLS["SUCCESS"] + " = " + self.COLS["R"]
-            valae = self.COLS["INFO"] + str(attr.value.value) + self.COLS["R"]
-            arrowpart = ""
-            if type(attr.children) == TraverseArrow:
-                arrowpart = " " + \
-                    self.COLS["WARNING"] + \
-                    "".join([str(" " + self.COLS["BLUE"] + self.charset["TraverseItem"]["TraverseArrow"] + self.COLS["CYAN"] +
-                            " %s") % v for v in attr.children.rights])
-            if attr.name == "body":
-                if hasattr(attr.o.body, "tokens"):
-                    valae = self.COLS["HEADER"] + attr.value[:5] + \
-                        (attr.value[5:] and "...") + \
-                        "["+len(attr.value)+"]" + self.COLS["R"]
-                    # attr.o.body.tokens
-                    arrowpart = " " + \
-                        self.COLS["WARNING"] + \
-                        " " + self.charset["TraverseItem"]["tokens"] + "(" + ",".join(attr.o.body.tokens) + ")"
-            return self.COLS["INFO2"] + self.charset["TraverseItem"]["Attr"] + self.COLS["SUCCESS"] + "Attr(" + namae + eqq + valae + self.COLS["SUCCESS"] + ")" + arrowpart + self.COLS["R"]
-
-    def get_text_of_TraverseArrow(self, arrow):
-        return str(arrow.value)
-
-
-TREE = LeftAligned
-
-
-def TREEBOX_E3LM(colorname, charset=[]):
-    """Return a BoxStyle for asciitree using ordered charset and named color"""
-    if charset == []:
-        # chr(0x2514), chr(0x2500), chr(0x2502), chr(0x251C)]
-        charset = ["└", "─", "│", "├"]
-
-    if colorname == "NONE":
-        box = {
-            'UP_AND_RIGHT': charset[0],
-            'HORIZONTAL': charset[1],
-            'VERTICAL': charset[2],
-            'VERTICAL_AND_RIGHT': charset[3],
-        }
-    else:
-        box = {
-            'UP_AND_RIGHT': COLORS[colorname] + charset[0] + COLORS["R"],
-            'HORIZONTAL': COLORS[colorname] + charset[1] + COLORS["R"],
-            'VERTICAL': COLORS[colorname] + charset[2] + COLORS["R"],
-            'VERTICAL_AND_RIGHT': COLORS[colorname] + charset[3] + COLORS["R"],
-        }
-    return box
-
-
-class BOXSTYLE(BoxStyle):
-    """A rendering style that uses box draw characters and a common layout."""
-    gfx = None        #: Glyphs to use.
-    color = "NONE"    #: Color to use for tree arrows.
-    label_space = 1   #: Space between glyphs and label.
-    horiz_len = 2     #: Length of horizontal lines
-    indent = 1        #: Indent for subtrees
-    label_format = u'{}'
-
-    def __init__(self, color="NONE", gfx=TREEBOX_E3LM, charset=[]):
-        self.color = color
-        self.gfx = gfx(color, charset)
-
-    def child_head(self, label):
-        return (' ' * self.indent
-                + self.gfx['VERTICAL_AND_RIGHT']
-                + self.gfx['HORIZONTAL'] * self.horiz_len
-                + ' ' * self.label_space
-                + label)
-
-    def child_tail(self, line):
-        return (' ' * self.indent
-                + self.gfx['VERTICAL']
-                + ' ' * self.horiz_len
-                + line)
-
-    def last_child_head(self, label):
-        return (' ' * self.indent
-                + self.gfx['UP_AND_RIGHT']
-                + self.gfx['HORIZONTAL'] * self.horiz_len
-                + ' ' * self.label_space
-                + label)
-
-    def last_child_tail(self, line):
-        return (' ' * self.indent
-                # + ' ' * len(self.gfx['VERTICAL'])
-                + ' ' * self.horiz_len
-                + line)
-
-
-TREE_NODES = TREE(draw=BOXSTYLE(color="INFO2", gfx=TREEBOX_E3LM, charset=[]))
-TREE_NODES_NC = TREE(draw=BOXSTYLE(color="NONE", gfx=TREEBOX_E3LM, charset=[]))
-TREE_NODES_NG = TREE(draw=BOXSTYLE(
-    color="INFO2", gfx=TREEBOX_E3LM, charset=["'->", "-", "|", "|->"]))
-TREE_NODES_NCNG = TREE(draw=BOXSTYLE(
-    color="NONE", gfx=TREEBOX_E3LM, charset=["'->", "-", "|", "|->"]))
-
-
-def _print(text, *args):  # pragma: no cover
-    _all = [str(text), ]
-    col = "ENDC"
-    for i, arg in enumerate(args):
-        if arg not in COLORS.keys():
-            _all.append(str(arg))
-        else:
-            col = arg
-
-    cprint("\n".join(_all), color=col)
-
-
-def cprint(text, color="NONE"):  # pragma: no cover
-    if color == "NONE" or color == "":
-        print(str(text))
-    else:
-        color = color.upper()
-        print(COLORS[color] + str(text) + COLORS["ENDC"])
-
-
-def nprint(node, max_level=6, treefunc=TREE_NODES, **kwargs):  # pragma: no cover
-    """Print nodes using `asciitree`"""
-
-    if "noglyph" in kwargs.keys():
-        if kwargs["noglyph"] == True:
-            traverse_charset = {
-                "Program": "*",
-                "Block": "o ",
-                "TraverseItem": {
-                    "Import": " < ",
-                    "Attr": "> ",
-                    "TraverseArrow": "=>",
-                    "tokens": "<=",
-                }
-            }
-
-            if treefunc == TREE_NODES:
-                treefunc = TREE_NODES_NG
-            elif treefunc == TREE_NODES_NC:
-                treefunc = TREE_NODES_NCNG
-        else:
-            traverse_charset = []
-    else:
-        traverse_charset = []
-
-    if "pallete" in kwargs.keys():
-        if kwargs["pallete"] == None:
-            pallete = {k: "" for k in COLORS.keys()}
-
-            if treefunc == TREE_NODES:
-                treefunc = TREE_NODES_NC
-            elif treefunc == TREE_NODES_NG:
-                treefunc = TREE_NODES_NCNG
-        else:
-            pallete = kwargs["pallete"]
-    else:
-        pallete = COLORS
-
-    treefunc.traverse = TRAVERSE(cols=pallete, charset=traverse_charset, **kwargs)
-    print("\n" + treefunc(node) + "\n")
+# -*- coding: utf-8 -*-
+
+from asciitree import LeftAligned, Traversal, KeyArgsConstructor
+from asciitree.drawing import BoxStyle
+
+COLORS = {
+    # Default...
+    "NONE": u"",
+    "HEADER": u'\x1b[95m',
+    "INFO": u'\x1b[38;5;164m',
+    "INFO2": u'\x1b[38;5;172m',
+    "SUCCESS": u'\x1b[38;5;173m',
+    "WARNING": u'\x1b[93m',
+    "BLACK": u'\x1b[30m',
+    "RED": u'\x1b[31m',
+    "GREEN": u'\x1b[32m',
+    "GREEN": u'\x1b[32m',
+    "YELLOW": u'\x1b[33m',
+    "BLUE": u'\x1b[34m',
+    "MAGENTA": u'\x1b[35m',
+    "CYAN": u'\x1b[36m',
+    "WHITE": u'\x1b[37m',
+    "DEFAULT": u'\x1b[39m',
+    "CYAN": u'\x1b[36m',
+    "BOLD": u'\x1b[1m',
+    "ITALICS": u'\x1b[3m',
+    "UNDERLINE": u'\x1b[4m',
+    "STRIKE": u'\x1b[9m',
+    "ENDC": u'\x1b[0m',
+    "R": u'\x1b[0m',
+    # From CLI...
+    "H": u'\x1b[95m',  # HEADER
+    "1": u'\x1b[38;5;164m',  # FIRST
+    "2": u'\x1b[38;5;173m',  # SECOND
+    "3": u'\x1b[38;5;177m',  # THIRD
+    "4": u'\x1b[38;5;225m',  # FOURTH
+    "E": u'\x1b[91m',  # ERROR
+    "W": u'\x1b[93m',  # WHITE
+    "R": u'\x1b[0m',  # RESET
+    "B": u'\x1b[1m',  # BOLD
+    "U": u'\x1b[4m',  # UNDERLINE
+
+    "RESET": u'\x1b[0m',
+    "GRAY": u'\x1b[38;5;245m',
+
+    "A": u'\x1b[38;5;164m',  # A
+    "B": u'\x1b[38;5;173m',  # B
+    "C": u'\x1b[38;5;177m',  # C
+    "D": u'\x1b[38;5;225m',  # D
+    "E": u'\x1b[95m',        # E
+    "LOG": u'\x1b[38;5;164m',  # LOGGING TAG
+    "LOG_MSG": u'\x1b[38;5;245m',  # LOGGING MESSAGE
+    "ERROR": u'\x1b[91m',  # ERROR
+}
+
+
+class TraverseArrow(KeyArgsConstructor):
+    pass
+
+
+class TraverseItem(KeyArgsConstructor):
+    pass
+
+
+class TRAVERSE(Traversal):
+    evaluate = False
+    program_name = ""
+
+    def __init__(self, cols=COLORS, charset=[], **kwargs):
+        self.charset = {
+            "Program": chr(4),
+            "Block": "□ ",
+            "TraverseItem": {
+                "Import": " ╰ ",
+                "Attr": "⌐ ",
+                "TraverseArrow": "→",
+                "tokens": "←",
+            },
+        } if charset == [] else charset
+        self.COLS = cols
+        super().__init__(**kwargs) # Pass kwargs to parent
+
+
+    def get_children(self, node):
+        """Return a list of children of a node."""
+        method = 'get_children_of_{}'.format(type(node).__name__)
+        getter = getattr(self, method, None)
+        if getter != None:
+            result = getter(node)
+            return result
+        return []
+
+    # Program node children
+    def get_children_of_Program(self, node):
+        imports = [TraverseItem(type="Import", value=x) for x in node.imports]
+        return [*imports, *node.blocks]
+
+    # Block node children (blocks + attrs + body)
+    def get_children_of_Block(self, block):
+        c = [
+            *block.children,
+            *[TraverseItem(type="Attr", name=a, o=block, value=b, children=self.get_children(b))
+              for a, b in block._attrs.items() if a != "body"],
+        ]
+        if hasattr(block, "body"):
+            c.append(TraverseItem(type="Attr", name="body",
+                     o=block, value=block._attrs["body"]))
+        return c
+
+    # Attr children (as arrows holder)
+    def get_children_of_Attr(self, attr):
+        if self.evaluate:
+            if hasattr(attr, "eval"):
+                return TraverseArrow(left=attr.value, rights=[
+                    f"\"{attr.eval}\"" if type(attr.eval) == str else attr.eval
+                ])
+        return [attr.value]
+
+    # Placeholder
+    def get_children_of_TraverseArrow(self, traverse_arrow):
+        return [*traverse_arrow.rights]
+
+    # Placeholder
+    def get_children_of_TraverseItem(self, traverse_item):
+        return []
+
+    def get_root(self, tree):
+        """Return a node representing the tree root from the tree."""
+        return tree
+
+    def get_text(self, node):
+        """Return the text associated with a node."""
+        method = 'get_text_of_{}'.format(type(node).__name__)
+        getter = getattr(self, method, None)
+        if getter != None:
+            result = getter(node)
+            return result
+        return str(node)
+
+    def get_text_of_Program(self, node):
+        namae = self.COLS["HEADER"] + self.program_name # or node.id
+        return self.COLS["BOLD"] + self.COLS["INFO2"] + " " + self.charset["Program"] + " " + self.COLS["INFO"] + "Program(" + namae + self.COLS["INFO"] + ")" + self.COLS["R"]
+
+    def get_text_of_Block(self, block):
+        idpart = (self.COLS["HEADER"] + self.COLS["UNDERLINE"] +
+                  f"#{block.id}" + self.COLS["R"]) if hasattr(block, "id") else ""
+        namepart = (self.COLS["HEADER"] + ", " + block.name +
+                    self.COLS["R"]) if block.name != "" else ""
+        namae = self.COLS["HEADER"] + block.type + idpart + namepart
+        return self.COLS["INFO2"]+ self.charset["Block"] + self.COLS["INFO"] + "Block(" + namae + self.COLS["INFO"] + ")" + self.COLS["R"]
+
+    def get_text_of_TraverseItem(self, item):
+        if item.type == "Import":
+            return self.COLS["INFO2"] + self.charset["TraverseItem"]["Import"] + self.COLS["GRAY"] + "import " + self.COLS["WHITE"] + item.value + self.COLS["R"]
+        elif item.type == "Attr":
+            attr = item
+            namae = self.COLS["HEADER"] + attr.name + self.COLS["R"]
+            eqq = self.COLS["SUCCESS"] + " = " + self.COLS["R"]
+            valae = self.COLS["INFO"] + str(attr.value.value) + self.COLS["R"]
+            arrowpart = ""
+            if type(attr.children) == TraverseArrow:
+                arrowpart = " " + \
+                    self.COLS["WARNING"] + \
+                    "".join([str(" " + self.COLS["BLUE"] + self.charset["TraverseItem"]["TraverseArrow"] + self.COLS["CYAN"] +
+                            " %s") % v for v in attr.children.rights])
+            if attr.name == "body":
+                if hasattr(attr.o.body, "tokens"):
+                    valae = self.COLS["HEADER"] + attr.value[:5] + \
+                        (attr.value[5:] and "...") + \
+                        "["+len(attr.value)+"]" + self.COLS["R"]
+                    # attr.o.body.tokens
+                    arrowpart = " " + \
+                        self.COLS["WARNING"] + \
+                        " " + self.charset["TraverseItem"]["tokens"] + "(" + ",".join(attr.o.body.tokens) + ")"
+            return self.COLS["INFO2"] + self.charset["TraverseItem"]["Attr"] + self.COLS["SUCCESS"] + "Attr(" + namae + eqq + valae + self.COLS["SUCCESS"] + ")" + arrowpart + self.COLS["R"]
+
+    def get_text_of_TraverseArrow(self, arrow):
+        return str(arrow.value)
+
+
+TREE = LeftAligned
+
+
+def TREEBOX_E3LM(colorname, charset=[]):
+    """Return a BoxStyle for asciitree using ordered charset and named color"""
+    if charset == []:
+        # chr(0x2514), chr(0x2500), chr(0x2502), chr(0x251C)]
+        charset = ["└", "─", "│", "├"]
+
+    if colorname == "NONE":
+        box = {
+            'UP_AND_RIGHT': charset[0],
+            'HORIZONTAL': charset[1],
+            'VERTICAL': charset[2],
+            'VERTICAL_AND_RIGHT': charset[3],
+        }
+    else:
+        box = {
+            'UP_AND_RIGHT': COLORS[colorname] + charset[0] + COLORS["R"],
+            'HORIZONTAL': COLORS[colorname] + charset[1] + COLORS["R"],
+            'VERTICAL': COLORS[colorname] + charset[2] + COLORS["R"],
+            'VERTICAL_AND_RIGHT': COLORS[colorname] + charset[3] + COLORS["R"],
+        }
+    return box
+
+
+class BOXSTYLE(BoxStyle):
+    """A rendering style that uses box draw characters and a common layout."""
+    gfx = None        #: Glyphs to use.
+    color = "NONE"    #: Color to use for tree arrows.
+    label_space = 1   #: Space between glyphs and label.
+    horiz_len = 2     #: Length of horizontal lines
+    indent = 1        #: Indent for subtrees
+    label_format = u'{}'
+
+    def __init__(self, color="NONE", gfx=TREEBOX_E3LM, charset=[]):
+        self.color = color
+        self.gfx = gfx(color, charset)
+
+    def child_head(self, label):
+        return (' ' * self.indent
+                + self.gfx['VERTICAL_AND_RIGHT']
+                + self.gfx['HORIZONTAL'] * self.horiz_len
+                + ' ' * self.label_space
+                + label)
+
+    def child_tail(self, line):
+        return (' ' * self.indent
+                + self.gfx['VERTICAL']
+                + ' ' * self.horiz_len
+                + line)
+
+    def last_child_head(self, label):
+        return (' ' * self.indent
+                + self.gfx['UP_AND_RIGHT']
+                + self.gfx['HORIZONTAL'] * self.horiz_len
+                + ' ' * self.label_space
+                + label)
+
+    def last_child_tail(self, line):
+        return (' ' * self.indent
+                # + ' ' * len(self.gfx['VERTICAL'])
+                + ' ' * self.horiz_len
+                + line)
+
+
+TREE_NODES = TREE(draw=BOXSTYLE(color="INFO2", gfx=TREEBOX_E3LM, charset=[]))
+TREE_NODES_NC = TREE(draw=BOXSTYLE(color="NONE", gfx=TREEBOX_E3LM, charset=[]))
+TREE_NODES_NG = TREE(draw=BOXSTYLE(
+    color="INFO2", gfx=TREEBOX_E3LM, charset=["'->", "-", "|", "|->"]))
+TREE_NODES_NCNG = TREE(draw=BOXSTYLE(
+    color="NONE", gfx=TREEBOX_E3LM, charset=["'->", "-", "|", "|->"]))
+
+
+def _print(text, *args):  # pragma: no cover
+    _all = [str(text), ]
+    col = "ENDC"
+    for i, arg in enumerate(args):
+        if arg not in COLORS.keys():
+            _all.append(str(arg))
+        else:
+            col = arg
+
+    cprint("\n".join(_all), color=col)
+
+
+def cprint(text, color="NONE"):  # pragma: no cover
+    if color == "NONE" or color == "":
+        print(str(text))
+    else:
+        color = color.upper()
+        print(COLORS[color] + str(text) + COLORS["ENDC"])
+
+
+def nprint(node, max_level=6, treefunc=TREE_NODES, **kwargs):  # pragma: no cover
+    """Print nodes using `asciitree`"""
+
+    if "noglyph" in kwargs.keys():
+        if kwargs["noglyph"] == True:
+            traverse_charset = {
+                "Program": "*",
+                "Block": "o ",
+                "TraverseItem": {
+                    "Import": " < ",
+                    "Attr": "> ",
+                    "TraverseArrow": "=>",
+                    "tokens": "<=",
+                }
+            }
+
+            if treefunc == TREE_NODES:
+                treefunc = TREE_NODES_NG
+            elif treefunc == TREE_NODES_NC:
+                treefunc = TREE_NODES_NCNG
+        else:
+            traverse_charset = []
+    else:
+        traverse_charset = []
+
+    if "pallete" in kwargs.keys():
+        if kwargs["pallete"] == None:
+            pallete = {k: "" for k in COLORS.keys()}
+
+            if treefunc == TREE_NODES:
+                treefunc = TREE_NODES_NC
+            elif treefunc == TREE_NODES_NG:
+                treefunc = TREE_NODES_NCNG
+        else:
+            pallete = kwargs["pallete"]
+    else:
+        pallete = COLORS
+
+    treefunc.traverse = TRAVERSE(cols=pallete, charset=traverse_charset, **kwargs)
+    print("\n" + treefunc(node) + "\n")
```

### Comparing `e3lm-0.1.8/src/e3lm/lang/interpreters.py` & `e3lm-0.1.9/src/e3lm/lang/interpreters.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,809 +1,809 @@
-"""
-Author: Kenan Masri
-
-"""
-import sys
-import functools
-from jinja2 import Template
-from e3lm.lang import ast
-from e3lm.lang.data import basic_dt
-from e3lm.helpers.printers import cprint
-
-stuck_counter = 0
-
-
-class InterpreterError(BaseException):
-    pass
-
-
-def get_attr(obj, attr):
-    """Return `attr` of `obj` by searching its `children`, `attrs` and actual
-    attributes in order."""
-    search = obj
-    if isinstance(obj, ast.AST):
-        if hasattr(obj, "eval") and obj.eval != None:
-            search = obj.eval
-
-    sattr = attr
-    if isinstance(attr, ast.AST):
-        if hasattr(attr, "eval") and attr.eval != None:
-            sattr = attr.eval
-
-    if isinstance(search, ast.AST):
-        if type(search) == ast.Identifier:
-            pass
-        if type(search) == ast.Program:
-            flat_blocks = search.flat_blocks
-            for fb in flat_blocks:
-                if sattr == fb.name:
-                    return fb
-
-    if isinstance(sattr, ast.AST):
-        if type(sattr) == ast.Block:
-            raise AttributeError
-
-    if type(search) in (list, dict, tuple, set):
-        try:
-            return search[sattr]
-        except (KeyError, ValueError):
-            return search[int(sattr)]
-
-    if hasattr(search, "children"):
-        names = [n.name for n in search.children]
-        if sattr in names:
-            return search.children[names.index(sattr)]
-
-    if hasattr(search, "_attrs"):
-        if sattr in search._attrs.keys():
-            return search._attrs[sattr]
-
-    if hasattr(search, sattr):
-        return getattr(search, sattr)
-
-    # Return empty body since it was not found.
-    if type(search) == ast.Block and attr == "body":
-        return ""
-
-    raise AttributeError("'{}' object has no attribute '{}'.".format(
-        search, attr
-    ))
-
-
-def dot_get(obj, attr, *args, **kwargs):
-    """Get `obj` nested `attr` in dotted syntax.
-
-    Available Keyword Arguments:
-        `eval` whether return evaluation or AST.
-
-    Examples:
-        dot_get(my_program, "dummy_1.attr2")
-        dot_get(my_program, "blocks.0.dummy_2")
-    """
-    if "eval" in kwargs.keys():
-        _eval = kwargs["eval"]
-    else:
-        _eval = False
-
-    def _getattr(obj, attr):
-        if hasattr(obj, "attrs"):
-            if attr in obj.attrs.keys():
-                return obj.attrs[attr] if _eval else obj._attrs[attr]
-        try:
-            if type(obj) in (list, dict, tuple, set):
-                try:
-                    return obj[int(attr)]
-                except (KeyError, ValueError):
-                    return obj[attr]
-        except ValueError:
-            raise AttributeError(f"{attr} was not found in {obj}")
-        try:
-            n = get_attr(obj, attr)
-        except AttributeError:
-            n = getattr(obj, attr, *args)
-        return n
-
-    dot = functools.reduce(_getattr, [obj] + attr.split('.'))
-    return dot
-
-
-class NodeVisitor:
-    """Base node visitor."""
-
-    def __init__(self):
-        self._idgen = 0
-
-    def id(self):
-        self._idgen += 1
-        return self._idgen - 1
-
-    def generic_visit(self, v):
-        return v
-
-    def visit(self, node):
-        """"""
-        if not hasattr(node, "_id") and type(node) not in ast.basic_dt:
-            node._id = self.id()
-
-        method = 'visit_{}'.format(type(node).__name__)
-        result = node
-        visitor = getattr(self, method, self.generic_visit)
-        if visitor == self.generic_visit:
-            raise NotImplementedError("No {} method.".format(method))
-        else:
-            result = visitor(result)
-        return result
-
-
-class Functions:
-    """Base class for functions."""
-    @staticmethod
-    def type_method(interpreter,
-                    inp=None, name="", args=[], **kwargs):
-        return getattr(inp, name)(*args)
-
-    @staticmethod
-    def prev(interpreter, *args, **kwargs):
-        klass = None
-        if len(args) > 0:
-            klass = args[0]
-        return interpreter.get_prev(klass, None)
-
-    @staticmethod
-    def next(interpreter, *args, **kwargs):
-        klass = None
-        if len(args) > 0:
-            klass = args[0]
-        return interpreter.get_next(klass, None)
-
-
-class E3lmInterpreter(NodeVisitor):
-    """Main E3lm Interpreter."""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        if "parser_kwargs" in kwargs.keys():
-            self.parser_kwargs = kwargs["parser_kwargs"]
-        else:
-            self.parser_kwargs = {}
-        if "parser" in kwargs.keys():
-            self.parser = kwargs["parser"]
-        else:
-            self.parser = None
-
-    def interpret(self, input, source=None):
-        if type(input) == str:
-            if self.parser:
-                tree = self.parser.parse(input, source, **self.parser_kwargs)
-            else:
-                raise Exception("Cannot interpret text without a parser.")
-        else:
-            tree = input
-        if tree == None:
-            return None
-        self.program = tree
-        # Here we visit all blocks and subblocks to append to the flat_blocks
-        # list for use later.
-        self.num_visit = 1
-        self.lazy_attrs = []
-        self.program = self.visit(self.program)
-        self.program.flat_blocks = self.flat_blocks
-        while len(self.lazy_attrs) > 0:
-            self.num_visit += 1
-            self.program = self.visit(self.program)
-        return self.program
-
-    def id(self):
-        """Generate an ID."""
-        self._idgen += 1
-        return self._idgen - 1
-
-    def visit(self, node, evaluate=False):
-        if node == None:
-            return None
-        if not hasattr(node, "_id") and type(node) not in ast.basic_dt:
-            node._id = self.id()
-
-        # Check if the object is provided as plugin.
-        is_plugin = False
-        if hasattr(self, "is_plugin"):
-            is_plugin = self.is_plugin
-
-        method = 'v_{}'.format(type(node).__name__)
-
-        result = node
-        visitor = getattr(self, method, self.generic_visit)
-        if visitor == self.generic_visit:
-            raise NotImplementedError("No {} method.".format(method))
-        else:
-            result = visitor(result, evaluate=evaluate)
-        return result
-
-    def get_next(self, klass=None, obj=None):
-        obj = obj or self.current_block
-
-        a = self.filter_flat(klass=klass)
-        if obj not in a:
-            n = 0
-        else:
-            n = a.index(obj) + 1
-        if klass:
-            for i in range(len(a)):
-                try:
-                    if a[n+i].type == klass:
-                        return a[n+i]
-                except IndexError:
-                    break
-        else:
-            if n >= len(a):
-                return None
-            try:
-                return a[n]
-            except IndexError:
-                raise RecursionError("Cannot get next({}) of object {}."
-                                     .format(str(klass), str(obj)))
-
-    def get_prev(self, klass=None, obj=None):
-        obj = obj or self.current_block
-        a = self.filter_flat(klass=klass)
-        if obj not in a:
-            n = 0
-        else:
-            n = a.index(obj) - 1
-        if klass:
-            for i in range(len(a)):
-                if n-i < 0:
-                    return None
-                try:
-                    if a[n-i].type == klass:
-                        return a[n-i]
-                except IndexError:
-                    break
-        else:
-            if n < 0:
-                return None
-            try:
-                return a[n]
-            except IndexError:
-                raise RecursionError("Cannot get prev({}) of object {}."
-                                     .format(str(klass), str(obj)))
-
-    def filter_flat(self, klass=None):
-        """Get `flat_blocks` filtered by `klass`."""
-        store = self.flat_blocks
-        if klass:
-            return [a for a in store if a.type == klass]
-        else:
-            return store
-
-    def abs_eval(self, obj, **kwargs):
-        """Return the absolute `eval` of `obj`"""
-        _types = (ast.Attr, ast.Identifier)
-        cblock = self.current_block
-        while type(obj) in _types:
-            if hasattr(obj, "eval"):
-                if type(obj) == ast.Attr:
-                    self.current_block = obj.parent
-                    if obj not in self.current_attr._eval:
-                        self.current_attr._eval.append(obj)
-                    obj = self.visit(obj, evaluate=2)
-                    if type(obj) in ast.basic_dt:
-                        break
-                if type(obj) == ast.Block:
-                    return obj
-                if obj.eval == None or obj.eval == obj:
-                    if obj not in self.current_attr._eval:
-                        self.current_attr._eval.append(obj)
-                    obj = self.visit(obj, evaluate=2)
-                    if type(obj) in ast.basic_dt:
-                        break
-                obj = obj.eval
-            else:
-                obj = self.visit(obj, evaluate=True)
-        self.current_block = cblock
-        if type(obj) not in _types:
-            obj = self.visit(obj, evaluate=True)
-        if obj not in self.current_attr._eval:
-            self.current_attr._eval.append(obj)
-        return obj
-
-    def v_Program(self, obj, *args, **kwargs):
-        self.current_block = None
-        if not hasattr(self, "flat_blocks"):
-            self.flat_blocks = []
-        if not hasattr(self, "_nav"):
-            self._nav = []
-
-        def add_to_nav(slf, b):
-            if b not in slf._nav:
-                slf._nav.append(b)
-                if len(b.children) > 0:
-                    for bb in b.children:
-                        add_to_nav(slf, bb)
-
-        for i, b in enumerate(obj.blocks):
-            add_to_nav(self, b)
-
-        for i, b in enumerate(obj.blocks):
-            obj.blocks[i] = b = self.visit(b, evaluate=True)
-
-        return obj
-
-    def v_Type(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        if evaluate:
-            obj.eval = obj.value
-            return obj.eval
-        return obj
-
-    def v_Block(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-        if not hasattr(obj, "parent"):
-            obj.parent = self.current_block or self.program
-
-        if not obj in self._nav:
-            self._nav.append(obj)
-
-        if obj not in self.flat_blocks:
-            self.flat_blocks.append(obj)
-
-        # Visit children blocks and then attributes.
-        for i, b in enumerate(obj.children):
-            self.current_block = obj
-            obj.children[i] = b = self.visit(b, evaluate=evaluate)
-
-        if not hasattr(obj, "attrs"):
-            obj.attrs = {}
-
-        for i, a in obj._attrs.items():
-            self.current_block = obj
-            self.current_attr = obj._attrs[i]
-            try:
-                obj._attrs[i] = self.visit(a, evaluate=True)
-            except RecursionError:
-                continue
-            self.current_block = obj
-            if evaluate != False:
-                self.current_attr = obj._attrs[i]
-                obj.attrs[i] = a.eval = self.visit(a, evaluate=2)
-
-        return obj
-
-    def v_Attr(self, obj, *args, **kwargs):
-        global stuck_counter  # For stack overflow avoidance
-        # --- RETURN BASED ON EVALUATE ---
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_lazy"):
-            obj._lazy = 1
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-        if not hasattr(obj, "parent"):
-            obj.parent = self.current_block
-        if not hasattr(obj, "_eval"):
-            obj._eval = []
-
-        if obj in self.lazy_attrs and obj._lazy == self.num_visit:
-            if self.current_attr not in self.lazy_attrs:
-                self.current_attr.lazy = self.num_visit
-                self.lazy_attrs.append(self.current_attr)
-            return ast.Lazy() if evaluate == 2 else obj
-
-        if obj.name == "body":
-            obj = self.v_body(obj, evaluate=False)
-            obj.eval = self.v_body(obj, evaluate=True)
-            obj._eval.append(obj.eval)
-            return obj.eval if evaluate == 2 else obj
-        else:
-            if len(obj._eval) >= 1 and type(obj._eval[-1]) == ast.Attr:
-                if obj.name == obj._eval[-1].name:
-                    raise RecursionError
-            try:
-                obj.value = self.visit(obj.value, evaluate=False)
-                _eval = self.visit(obj.value, evaluate=2)
-                if _eval not in obj._eval:
-                    obj._eval.append(_eval)
-
-                obj.eval = self.abs_eval(_eval)
-                if obj in self.lazy_attrs:
-                    self.lazy_attrs.remove(obj)
-
-                # Removed recursion limit for 3lm interpreter..
-                # Basically a 3lm file won't be that large.
-
-                # stuck_counter += 1
-                # if stuck_counter > sys.getrecursionlimit():
-                    # print("Stuck at recursion: " + str(stuck_counter) + "\nThe attribute", obj, "is bugged. Please check your 3lm code.")
-                    # stuck_counter = 0
-                    # exit(1)
-
-                return obj.eval if evaluate == 2 else obj
-            except (AttributeError, ValueError) as e:
-                if obj not in self.lazy_attrs:
-                    obj.lazy = self.num_visit
-                    self.lazy_attrs.append(obj)
-                return obj
-
-    # TODO better Jinja2 implementation
-    def v_body(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if evaluate:
-            if not hasattr(obj, "_body_template"):
-                val = obj.value
-                if isinstance(val, ast.Str):
-                    val = str(val.value)
-                obj._body_template = Template(val)
-            kwargs = self.current_block.attrs
-            if isinstance(obj, ast.Attr):
-                obj.tokens = []
-            kwargs = {**kwargs, "tokens": obj.tokens}
-            obj.eval = obj._body_template.render(**kwargs)
-            return obj.eval if evaluate else obj
-        # return obj
-        # obj.eval = obj.value
-        return obj.eval if evaluate else obj
-
-    def v_Identifier(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        for i, a in enumerate(obj.children):
-            obj.children[i] = a = self.visit(a, evaluate=False)
-            if isinstance(obj.children[i], ast.AST):
-                if type(obj.children[i]) not in (ast.Block,):
-                    obj.children[i].eval = self.visit(a, evaluate=True)
-
-        c = None  # current child
-        a = None  # child
-        skip = False
-        for i, a in enumerate(obj.children):
-            if skip:
-                skip = False
-                continue
-            b = obj.children[i+1] if i+1 < len(obj.children) else None
-            if b != None:
-                _d = False  # Whether done tests.
-                # If func, get the argument before and do it as an attribute.
-                if type(b) == ast.Func:
-                    # Visit arguments:
-                    fname = b.value  # e.g. split
-                    inp = self.abs_eval(a)
-                    ch = [self.abs_eval(_c) for _c in b.children]
-                    try:
-                        test = Functions.type_method(self,
-                                                     inp=inp, name=fname,
-                                                     args=ch)
-                        _d = True
-                    except AttributeError as e:
-                        raise e from None
-                else:
-                    # Try the attribute method.
-                    bb = b.eval if hasattr(b, "eval") else b
-                    aa = a.eval if hasattr(a, "eval") else a
-                    if aa == None:
-                        raise AttributeError(f"None does not have {bb}")
-                    try:
-                        if c == None:
-                            _c = self.current_block
-                            c = _c
-                        else:
-                            _c = self.abs_eval(c)
-                        test = get_attr(_c, aa)
-                        c = test
-                        obj.eval = c
-                        _d = False  # Do not skip
-                    except AttributeError:
-                        try:
-                            test = get_attr(aa, bb)
-                            obj.eval = test
-                            c = test
-                            _d = True
-                        except AttributeError as e:
-                            # Try the local/global keyword
-                            arr = [(_b.name, _b.type)
-                                   for _b in self.flat_blocks]
-                            try:
-                                ar = [k[0] for k in arr]
-                                test = self.flat_blocks[ar.index(aa)]
-                                c = test
-                                obj.eval = test
-                                _d = False
-                            except ValueError:
-                                try:
-                                    ar = [k[1] for k in arr]
-                                    test = self.flat_blocks[ar.index(aa)].type
-                                    obj.eval = test
-                                    _d = False
-                                except ValueError:
-                                    raise AttributeError(
-                                        "keyword '{}' does not exist.".format(
-                                            aa
-                                        ))
-                if _d:
-                    obj.eval = test
-                    skip = True
-            else:
-                _d = False
-                aa = a.eval if hasattr(a, "eval") else a
-                # Try the local/global keyword
-                try:
-                    if c == None:
-                        c = self.current_block
-                    test = get_attr(c, aa)
-                    c = test
-                    obj.eval = c
-                    _d = False  # Do not skip
-                except AttributeError:
-                    arr = [(_b.name, _b.type)
-                           for _b in self._nav]
-                    try:
-                        ar = [k[1] for k in arr]
-                        test = self._nav[ar.index(aa)].type
-                        obj.eval = test
-                        _d = False
-                    except ValueError:
-                        try:
-                            ar = [k[0] for k in arr]
-                            test = self._nav[ar.index(aa)]
-                            c = test
-                            obj.eval = test
-                            _d = False
-                        except ValueError:
-                            # Check if aa does not exist as global block
-                            ar = [k.name for k in self._nav]
-                            ar2 = [k.type for k in self._nav]
-                            if aa not in ar:
-                                print(ar)
-                                if aa not in ar2:
-                                    raise InterpreterError(
-                                        f"{c} does not have {aa}."
-                                    ) from None
-                                else:
-                                    test = self._nav[ar.index(aa)].type
-                                    obj.eval = test
-                                    _d = False
-                            else:
-                                # Check if aa does not exist on block/attr
-                                if type(c) == ast.Attr:
-                                    c = c._eval[0]
-                                if aa not in c.attrs:
-                                    test = self._nav[ar.index(aa)]
-                                    obj.eval = test
-                                    _d = False
-                                else:
-                                    raise AttributeError(
-                                        "keyword '{}' does not exist.".format(
-                                            aa
-                                        )) from None
-
-                if _d:
-                    obj.eval = test
-                    if type(obj.eval) == ast.Attr:
-                        obj.target = obj.eval
-                        obj.eval = self.visit(obj.eval, evaluate=2)
-        if not hasattr(obj, "eval"):
-            raise SyntaxError("keyword '" + str(obj.children[0])
-                              + "' is unknown.") from None
-
-        return obj.eval if evaluate else obj
-
-    def v_Index(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        obj.eval = self.visit(obj.value, evaluate=True)
-        return obj.eval if evaluate else obj
-
-    def v_UnaryOp(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        op = obj.op
-        ev = self.visit(obj.value, evaluate=True)
-        while (type(ev) not in ast.basic_dt):
-            ev = self.abs_eval(ev)
-
-        if op == "+":
-            obj.eval = + ev
-        elif op == "-":
-            obj.eval = - ev
-        return obj.eval if evaluate else obj
-
-    def v_BinOp(self, obj, *args, **kwargs):
-
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        leval = self.visit(obj.left, evaluate=True)
-        reval = self.visit(obj.right, evaluate=True)
-
-        while (type(leval) not in ast.basic_dt) \
-                or (type(reval) not in ast.basic_dt):
-            leval = self.abs_eval(leval)
-            reval = self.abs_eval(reval)
-
-        try:
-            if obj.op == "+":
-                obj.eval = leval + reval
-            elif obj.op == "-":
-                obj.eval = leval - reval
-            elif obj.op == "*":
-                obj.eval = leval * reval
-            elif obj.op == "/":
-                obj.eval = leval / reval
-            elif obj.op == "**":
-                obj.eval = leval ** reval
-            elif obj.op == "//":
-                obj.eval = leval // reval
-        except TypeError as e:
-            raise TypeError("attr '"
-                            + str(self.current_attr.name) + "' in block '"
-                            + str(self.current_block) + "' invalid "
-                            + str(obj) + ".")
-        return obj.eval if evaluate else obj
-
-    def v_Num(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        obj.eval = obj.value
-        if obj.type == "NUM_FLOAT":
-            obj.eval = float(obj.value)
-        elif obj.type == "NUM_OCT":
-            obj.eval = int(obj.value, base=8)
-        elif obj.type == "NUM_BIN":
-            obj.eval = int(obj.value, base=2)
-        elif obj.type == "NUM_HEX":
-            obj.eval = int(obj.value, base=16)
-        elif obj.type == "NUM_IMAG":
-            obj.eval = obj.value[0]
-        return obj.eval if evaluate else obj
-
-    def v_Str(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        # Convert to a Type if it means a type literal.
-        # if obj.value in [b.type for b in self.flat_blocks]:
-        #     obj = ast.Type(obj.value)
-
-        obj.eval = self.visit(obj.value, evaluate=True)
-        return obj.eval if evaluate else obj
-
-    def v_Bool(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        obj.eval = self.visit(obj.value, evaluate=True)
-        return obj.eval if evaluate else obj
-
-    def v_Undefined(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-        obj.eval = self.visit(obj.value, evaluate=True)
-        return obj.eval if evaluate else obj
-
-    def v_obj(self, obj, *args, **kwargs):
-        return obj
-
-    def v_dict(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if evaluate:
-            return {self.visit(key, evaluate=True): self.visit(val)
-                    for key, val in obj.items()}
-        else:
-            return {self.visit(key, evaluate=False): self.visit(
-                val, evaluate=False) for key, val in obj.items()}
-
-    def v_list(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        return [self.visit(val, evaluate=evaluate) for val in obj]
-
-    v_str = v_obj
-    v_int = v_obj
-    v_float = v_obj
-    v_tuple = v_obj
-    v_complex = v_obj
-    v_bool = v_obj
-
-    def v_Array(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        _ar = []
-        for a in obj.children:
-            a = self.visit(a, evaluate=True)
-            if hasattr(a, "eval"):
-                a = a.eval
-            _ar.append(a)
-        obj.eval = _ar
-        return obj.eval if evaluate else obj
-
-    def v_Dict(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        _dict = {}
-        for cpl in obj.children:
-            cpl.left = self.visit(cpl.left, evaluate=True)
-            cpl.right = self.visit(cpl.right, evaluate=True)
-            cpl_left = cpl.left.eval \
-                if "eval" in dir(cpl.left) else cpl.left
-            cpl_right = cpl.right.eval \
-                if "eval" in dir(cpl.right) else cpl.right
-            _dict[cpl_left] = cpl_right
-        obj.eval = _dict
-        return obj.eval if evaluate else obj
-
-    def v_Func(self, obj, *args, **kwargs):
-        evaluate = kwargs["evaluate"]
-        if not hasattr(obj, "_id"):
-            obj._id = self.id()
-
-        for i, a in enumerate(obj.children):
-            a.eval = self.visit(a, evaluate=True)
-            obj.children[i] = a
-
-        fname = self.visit(obj.value, evaluate=True)
-
-        obj.call = getattr(Functions,
-                           fname, None)
-        if obj.call:
-            obj.eval = obj.call(self, *[a.eval for a in obj.children])
-        else:
-            return obj
-        return obj.eval if evaluate else obj
-
-
-class E3lmPlugin(E3lmInterpreter):
-    """Base class for an E3lm interpretation plugin.
-
-    `options` must contain a "key" that indicates what attribute to
-    assign to the program.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.options = kwargs
-        self.is_plugin = True
-
-    def interpret(self, input, source=None):
-        self.program = input
-        new_data = self.visit(self.program)
-        if "key" in self.options.keys():
-            attr = self.options["key"]
-        else:
-            raise NotImplementedError("Interpret is not implemented properly.")
-        setattr(self.program, attr, new_data)
-        return self.program
-
-    def v_Program(self, obj, *args, **kwargs):
-        for i, b in enumerate(obj.blocks):
-            b = self.visit(b)
-        return obj
-
-    def v_Block(self, obj, *args, **kwargs):
-        ast = False
-        if "ast" in self.options.keys():
-            ast = self.options["ast"]
-
-        for i, b in enumerate(obj.children):
-            b = self.visit(b)
-
-        for i, b in enumerate(obj.attrs):
-            b = self.visit(b)
-
-        return obj
+"""
+Author: Kenan Masri
+
+"""
+import sys
+import functools
+from jinja2 import Template
+from e3lm.lang import ast
+from e3lm.lang.data import basic_dt
+from e3lm.helpers.printers import cprint
+
+stuck_counter = 0
+
+
+class InterpreterError(BaseException):
+    pass
+
+
+def get_attr(obj, attr):
+    """Return `attr` of `obj` by searching its `children`, `attrs` and actual
+    attributes in order."""
+    search = obj
+    if isinstance(obj, ast.AST):
+        if hasattr(obj, "eval") and obj.eval != None:
+            search = obj.eval
+
+    sattr = attr
+    if isinstance(attr, ast.AST):
+        if hasattr(attr, "eval") and attr.eval != None:
+            sattr = attr.eval
+
+    if isinstance(search, ast.AST):
+        if type(search) == ast.Identifier:
+            pass
+        if type(search) == ast.Program:
+            flat_blocks = search.flat_blocks
+            for fb in flat_blocks:
+                if sattr == fb.name:
+                    return fb
+
+    if isinstance(sattr, ast.AST):
+        if type(sattr) == ast.Block:
+            raise AttributeError
+
+    if type(search) in (list, dict, tuple, set):
+        try:
+            return search[sattr]
+        except (KeyError, ValueError):
+            return search[int(sattr)]
+
+    if hasattr(search, "children"):
+        names = [n.name for n in search.children]
+        if sattr in names:
+            return search.children[names.index(sattr)]
+
+    if hasattr(search, "_attrs"):
+        if sattr in search._attrs.keys():
+            return search._attrs[sattr]
+
+    if hasattr(search, sattr):
+        return getattr(search, sattr)
+
+    # Return empty body since it was not found.
+    if type(search) == ast.Block and attr == "body":
+        return ""
+
+    raise AttributeError("'{}' object has no attribute '{}'.".format(
+        search, attr
+    ))
+
+
+def dot_get(obj, attr, *args, **kwargs):
+    """Get `obj` nested `attr` in dotted syntax.
+
+    Available Keyword Arguments:
+        `eval` whether return evaluation or AST.
+
+    Examples:
+        dot_get(my_program, "dummy_1.attr2")
+        dot_get(my_program, "blocks.0.dummy_2")
+    """
+    if "eval" in kwargs.keys():
+        _eval = kwargs["eval"]
+    else:
+        _eval = False
+
+    def _getattr(obj, attr):
+        if hasattr(obj, "attrs"):
+            if attr in obj.attrs.keys():
+                return obj.attrs[attr] if _eval else obj._attrs[attr]
+        try:
+            if type(obj) in (list, dict, tuple, set):
+                try:
+                    return obj[int(attr)]
+                except (KeyError, ValueError):
+                    return obj[attr]
+        except ValueError:
+            raise AttributeError(f"{attr} was not found in {obj}")
+        try:
+            n = get_attr(obj, attr)
+        except AttributeError:
+            n = getattr(obj, attr, *args)
+        return n
+
+    dot = functools.reduce(_getattr, [obj] + attr.split('.'))
+    return dot
+
+
+class NodeVisitor:
+    """Base node visitor."""
+
+    def __init__(self):
+        self._idgen = 0
+
+    def id(self):
+        self._idgen += 1
+        return self._idgen - 1
+
+    def generic_visit(self, v):
+        return v
+
+    def visit(self, node):
+        """"""
+        if not hasattr(node, "_id") and type(node) not in ast.basic_dt:
+            node._id = self.id()
+
+        method = 'visit_{}'.format(type(node).__name__)
+        result = node
+        visitor = getattr(self, method, self.generic_visit)
+        if visitor == self.generic_visit:
+            raise NotImplementedError("No {} method.".format(method))
+        else:
+            result = visitor(result)
+        return result
+
+
+class Functions:
+    """Base class for functions."""
+    @staticmethod
+    def type_method(interpreter,
+                    inp=None, name="", args=[], **kwargs):
+        return getattr(inp, name)(*args)
+
+    @staticmethod
+    def prev(interpreter, *args, **kwargs):
+        klass = None
+        if len(args) > 0:
+            klass = args[0]
+        return interpreter.get_prev(klass, None)
+
+    @staticmethod
+    def next(interpreter, *args, **kwargs):
+        klass = None
+        if len(args) > 0:
+            klass = args[0]
+        return interpreter.get_next(klass, None)
+
+
+class E3lmInterpreter(NodeVisitor):
+    """Main E3lm Interpreter."""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        if "parser_kwargs" in kwargs.keys():
+            self.parser_kwargs = kwargs["parser_kwargs"]
+        else:
+            self.parser_kwargs = {}
+        if "parser" in kwargs.keys():
+            self.parser = kwargs["parser"]
+        else:
+            self.parser = None
+
+    def interpret(self, input, source=None):
+        if type(input) == str:
+            if self.parser:
+                tree = self.parser.parse(input, source, **self.parser_kwargs)
+            else:
+                raise Exception("Cannot interpret text without a parser.")
+        else:
+            tree = input
+        if tree == None:
+            return None
+        self.program = tree
+        # Here we visit all blocks and subblocks to append to the flat_blocks
+        # list for use later.
+        self.num_visit = 1
+        self.lazy_attrs = []
+        self.program = self.visit(self.program)
+        self.program.flat_blocks = self.flat_blocks
+        while len(self.lazy_attrs) > 0:
+            self.num_visit += 1
+            self.program = self.visit(self.program)
+        return self.program
+
+    def id(self):
+        """Generate an ID."""
+        self._idgen += 1
+        return self._idgen - 1
+
+    def visit(self, node, evaluate=False):
+        if node == None:
+            return None
+        if not hasattr(node, "_id") and type(node) not in ast.basic_dt:
+            node._id = self.id()
+
+        # Check if the object is provided as plugin.
+        is_plugin = False
+        if hasattr(self, "is_plugin"):
+            is_plugin = self.is_plugin
+
+        method = 'v_{}'.format(type(node).__name__)
+
+        result = node
+        visitor = getattr(self, method, self.generic_visit)
+        if visitor == self.generic_visit:
+            raise NotImplementedError("No {} method.".format(method))
+        else:
+            result = visitor(result, evaluate=evaluate)
+        return result
+
+    def get_next(self, klass=None, obj=None):
+        obj = obj or self.current_block
+
+        a = self.filter_flat(klass=klass)
+        if obj not in a:
+            n = 0
+        else:
+            n = a.index(obj) + 1
+        if klass:
+            for i in range(len(a)):
+                try:
+                    if a[n+i].type == klass:
+                        return a[n+i]
+                except IndexError:
+                    break
+        else:
+            if n >= len(a):
+                return None
+            try:
+                return a[n]
+            except IndexError:
+                raise RecursionError("Cannot get next({}) of object {}."
+                                     .format(str(klass), str(obj)))
+
+    def get_prev(self, klass=None, obj=None):
+        obj = obj or self.current_block
+        a = self.filter_flat(klass=klass)
+        if obj not in a:
+            n = 0
+        else:
+            n = a.index(obj) - 1
+        if klass:
+            for i in range(len(a)):
+                if n-i < 0:
+                    return None
+                try:
+                    if a[n-i].type == klass:
+                        return a[n-i]
+                except IndexError:
+                    break
+        else:
+            if n < 0:
+                return None
+            try:
+                return a[n]
+            except IndexError:
+                raise RecursionError("Cannot get prev({}) of object {}."
+                                     .format(str(klass), str(obj)))
+
+    def filter_flat(self, klass=None):
+        """Get `flat_blocks` filtered by `klass`."""
+        store = self.flat_blocks
+        if klass:
+            return [a for a in store if a.type == klass]
+        else:
+            return store
+
+    def abs_eval(self, obj, **kwargs):
+        """Return the absolute `eval` of `obj`"""
+        _types = (ast.Attr, ast.Identifier)
+        cblock = self.current_block
+        while type(obj) in _types:
+            if hasattr(obj, "eval"):
+                if type(obj) == ast.Attr:
+                    self.current_block = obj.parent
+                    if obj not in self.current_attr._eval:
+                        self.current_attr._eval.append(obj)
+                    obj = self.visit(obj, evaluate=2)
+                    if type(obj) in ast.basic_dt:
+                        break
+                if type(obj) == ast.Block:
+                    return obj
+                if obj.eval == None or obj.eval == obj:
+                    if obj not in self.current_attr._eval:
+                        self.current_attr._eval.append(obj)
+                    obj = self.visit(obj, evaluate=2)
+                    if type(obj) in ast.basic_dt:
+                        break
+                obj = obj.eval
+            else:
+                obj = self.visit(obj, evaluate=True)
+        self.current_block = cblock
+        if type(obj) not in _types:
+            obj = self.visit(obj, evaluate=True)
+        if obj not in self.current_attr._eval:
+            self.current_attr._eval.append(obj)
+        return obj
+
+    def v_Program(self, obj, *args, **kwargs):
+        self.current_block = None
+        if not hasattr(self, "flat_blocks"):
+            self.flat_blocks = []
+        if not hasattr(self, "_nav"):
+            self._nav = []
+
+        def add_to_nav(slf, b):
+            if b not in slf._nav:
+                slf._nav.append(b)
+                if len(b.children) > 0:
+                    for bb in b.children:
+                        add_to_nav(slf, bb)
+
+        for i, b in enumerate(obj.blocks):
+            add_to_nav(self, b)
+
+        for i, b in enumerate(obj.blocks):
+            obj.blocks[i] = b = self.visit(b, evaluate=True)
+
+        return obj
+
+    def v_Type(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        if evaluate:
+            obj.eval = obj.value
+            return obj.eval
+        return obj
+
+    def v_Block(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+        if not hasattr(obj, "parent"):
+            obj.parent = self.current_block or self.program
+
+        if not obj in self._nav:
+            self._nav.append(obj)
+
+        if obj not in self.flat_blocks:
+            self.flat_blocks.append(obj)
+
+        # Visit children blocks and then attributes.
+        for i, b in enumerate(obj.children):
+            self.current_block = obj
+            obj.children[i] = b = self.visit(b, evaluate=evaluate)
+
+        if not hasattr(obj, "attrs"):
+            obj.attrs = {}
+
+        for i, a in obj._attrs.items():
+            self.current_block = obj
+            self.current_attr = obj._attrs[i]
+            try:
+                obj._attrs[i] = self.visit(a, evaluate=True)
+            except RecursionError:
+                continue
+            self.current_block = obj
+            if evaluate != False:
+                self.current_attr = obj._attrs[i]
+                obj.attrs[i] = a.eval = self.visit(a, evaluate=2)
+
+        return obj
+
+    def v_Attr(self, obj, *args, **kwargs):
+        global stuck_counter  # For stack overflow avoidance
+        # --- RETURN BASED ON EVALUATE ---
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_lazy"):
+            obj._lazy = 1
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+        if not hasattr(obj, "parent"):
+            obj.parent = self.current_block
+        if not hasattr(obj, "_eval"):
+            obj._eval = []
+
+        if obj in self.lazy_attrs and obj._lazy == self.num_visit:
+            if self.current_attr not in self.lazy_attrs:
+                self.current_attr.lazy = self.num_visit
+                self.lazy_attrs.append(self.current_attr)
+            return ast.Lazy() if evaluate == 2 else obj
+
+        if obj.name == "body":
+            obj = self.v_body(obj, evaluate=False)
+            obj.eval = self.v_body(obj, evaluate=True)
+            obj._eval.append(obj.eval)
+            return obj.eval if evaluate == 2 else obj
+        else:
+            if len(obj._eval) >= 1 and type(obj._eval[-1]) == ast.Attr:
+                if obj.name == obj._eval[-1].name:
+                    raise RecursionError
+            try:
+                obj.value = self.visit(obj.value, evaluate=False)
+                _eval = self.visit(obj.value, evaluate=2)
+                if _eval not in obj._eval:
+                    obj._eval.append(_eval)
+
+                obj.eval = self.abs_eval(_eval)
+                if obj in self.lazy_attrs:
+                    self.lazy_attrs.remove(obj)
+
+                # Removed recursion limit for 3lm interpreter..
+                # Basically a 3lm file won't be that large.
+
+                # stuck_counter += 1
+                # if stuck_counter > sys.getrecursionlimit():
+                    # print("Stuck at recursion: " + str(stuck_counter) + "\nThe attribute", obj, "is bugged. Please check your 3lm code.")
+                    # stuck_counter = 0
+                    # exit(1)
+
+                return obj.eval if evaluate == 2 else obj
+            except (AttributeError, ValueError) as e:
+                if obj not in self.lazy_attrs:
+                    obj.lazy = self.num_visit
+                    self.lazy_attrs.append(obj)
+                return obj
+
+    # TODO better Jinja2 implementation
+    def v_body(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if evaluate:
+            if not hasattr(obj, "_body_template"):
+                val = obj.value
+                if isinstance(val, ast.Str):
+                    val = str(val.value)
+                obj._body_template = Template(val)
+            kwargs = self.current_block.attrs
+            if isinstance(obj, ast.Attr):
+                obj.tokens = []
+            kwargs = {**kwargs, "tokens": obj.tokens}
+            obj.eval = obj._body_template.render(**kwargs)
+            return obj.eval if evaluate else obj
+        # return obj
+        # obj.eval = obj.value
+        return obj.eval if evaluate else obj
+
+    def v_Identifier(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        for i, a in enumerate(obj.children):
+            obj.children[i] = a = self.visit(a, evaluate=False)
+            if isinstance(obj.children[i], ast.AST):
+                if type(obj.children[i]) not in (ast.Block,):
+                    obj.children[i].eval = self.visit(a, evaluate=True)
+
+        c = None  # current child
+        a = None  # child
+        skip = False
+        for i, a in enumerate(obj.children):
+            if skip:
+                skip = False
+                continue
+            b = obj.children[i+1] if i+1 < len(obj.children) else None
+            if b != None:
+                _d = False  # Whether done tests.
+                # If func, get the argument before and do it as an attribute.
+                if type(b) == ast.Func:
+                    # Visit arguments:
+                    fname = b.value  # e.g. split
+                    inp = self.abs_eval(a)
+                    ch = [self.abs_eval(_c) for _c in b.children]
+                    try:
+                        test = Functions.type_method(self,
+                                                     inp=inp, name=fname,
+                                                     args=ch)
+                        _d = True
+                    except AttributeError as e:
+                        raise e from None
+                else:
+                    # Try the attribute method.
+                    bb = b.eval if hasattr(b, "eval") else b
+                    aa = a.eval if hasattr(a, "eval") else a
+                    if aa == None:
+                        raise AttributeError(f"None does not have {bb}")
+                    try:
+                        if c == None:
+                            _c = self.current_block
+                            c = _c
+                        else:
+                            _c = self.abs_eval(c)
+                        test = get_attr(_c, aa)
+                        c = test
+                        obj.eval = c
+                        _d = False  # Do not skip
+                    except AttributeError:
+                        try:
+                            test = get_attr(aa, bb)
+                            obj.eval = test
+                            c = test
+                            _d = True
+                        except AttributeError as e:
+                            # Try the local/global keyword
+                            arr = [(_b.name, _b.type)
+                                   for _b in self.flat_blocks]
+                            try:
+                                ar = [k[0] for k in arr]
+                                test = self.flat_blocks[ar.index(aa)]
+                                c = test
+                                obj.eval = test
+                                _d = False
+                            except ValueError:
+                                try:
+                                    ar = [k[1] for k in arr]
+                                    test = self.flat_blocks[ar.index(aa)].type
+                                    obj.eval = test
+                                    _d = False
+                                except ValueError:
+                                    raise AttributeError(
+                                        "keyword '{}' does not exist.".format(
+                                            aa
+                                        ))
+                if _d:
+                    obj.eval = test
+                    skip = True
+            else:
+                _d = False
+                aa = a.eval if hasattr(a, "eval") else a
+                # Try the local/global keyword
+                try:
+                    if c == None:
+                        c = self.current_block
+                    test = get_attr(c, aa)
+                    c = test
+                    obj.eval = c
+                    _d = False  # Do not skip
+                except AttributeError:
+                    arr = [(_b.name, _b.type)
+                           for _b in self._nav]
+                    try:
+                        ar = [k[1] for k in arr]
+                        test = self._nav[ar.index(aa)].type
+                        obj.eval = test
+                        _d = False
+                    except ValueError:
+                        try:
+                            ar = [k[0] for k in arr]
+                            test = self._nav[ar.index(aa)]
+                            c = test
+                            obj.eval = test
+                            _d = False
+                        except ValueError:
+                            # Check if aa does not exist as global block
+                            ar = [k.name for k in self._nav]
+                            ar2 = [k.type for k in self._nav]
+                            if aa not in ar:
+                                print(ar)
+                                if aa not in ar2:
+                                    raise InterpreterError(
+                                        f"{c} does not have {aa}."
+                                    ) from None
+                                else:
+                                    test = self._nav[ar.index(aa)].type
+                                    obj.eval = test
+                                    _d = False
+                            else:
+                                # Check if aa does not exist on block/attr
+                                if type(c) == ast.Attr:
+                                    c = c._eval[0]
+                                if aa not in c.attrs:
+                                    test = self._nav[ar.index(aa)]
+                                    obj.eval = test
+                                    _d = False
+                                else:
+                                    raise AttributeError(
+                                        "keyword '{}' does not exist.".format(
+                                            aa
+                                        )) from None
+
+                if _d:
+                    obj.eval = test
+                    if type(obj.eval) == ast.Attr:
+                        obj.target = obj.eval
+                        obj.eval = self.visit(obj.eval, evaluate=2)
+        if not hasattr(obj, "eval"):
+            raise SyntaxError("keyword '" + str(obj.children[0])
+                              + "' is unknown.") from None
+
+        return obj.eval if evaluate else obj
+
+    def v_Index(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        obj.eval = self.visit(obj.value, evaluate=True)
+        return obj.eval if evaluate else obj
+
+    def v_UnaryOp(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        op = obj.op
+        ev = self.visit(obj.value, evaluate=True)
+        while (type(ev) not in ast.basic_dt):
+            ev = self.abs_eval(ev)
+
+        if op == "+":
+            obj.eval = + ev
+        elif op == "-":
+            obj.eval = - ev
+        return obj.eval if evaluate else obj
+
+    def v_BinOp(self, obj, *args, **kwargs):
+
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        leval = self.visit(obj.left, evaluate=True)
+        reval = self.visit(obj.right, evaluate=True)
+
+        while (type(leval) not in ast.basic_dt) \
+                or (type(reval) not in ast.basic_dt):
+            leval = self.abs_eval(leval)
+            reval = self.abs_eval(reval)
+
+        try:
+            if obj.op == "+":
+                obj.eval = leval + reval
+            elif obj.op == "-":
+                obj.eval = leval - reval
+            elif obj.op == "*":
+                obj.eval = leval * reval
+            elif obj.op == "/":
+                obj.eval = leval / reval
+            elif obj.op == "**":
+                obj.eval = leval ** reval
+            elif obj.op == "//":
+                obj.eval = leval // reval
+        except TypeError as e:
+            raise TypeError("attr '"
+                            + str(self.current_attr.name) + "' in block '"
+                            + str(self.current_block) + "' invalid "
+                            + str(obj) + ".")
+        return obj.eval if evaluate else obj
+
+    def v_Num(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        obj.eval = obj.value
+        if obj.type == "NUM_FLOAT":
+            obj.eval = float(obj.value)
+        elif obj.type == "NUM_OCT":
+            obj.eval = int(obj.value, base=8)
+        elif obj.type == "NUM_BIN":
+            obj.eval = int(obj.value, base=2)
+        elif obj.type == "NUM_HEX":
+            obj.eval = int(obj.value, base=16)
+        elif obj.type == "NUM_IMAG":
+            obj.eval = obj.value[0]
+        return obj.eval if evaluate else obj
+
+    def v_Str(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        # Convert to a Type if it means a type literal.
+        # if obj.value in [b.type for b in self.flat_blocks]:
+        #     obj = ast.Type(obj.value)
+
+        obj.eval = self.visit(obj.value, evaluate=True)
+        return obj.eval if evaluate else obj
+
+    def v_Bool(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        obj.eval = self.visit(obj.value, evaluate=True)
+        return obj.eval if evaluate else obj
+
+    def v_Undefined(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+        obj.eval = self.visit(obj.value, evaluate=True)
+        return obj.eval if evaluate else obj
+
+    def v_obj(self, obj, *args, **kwargs):
+        return obj
+
+    def v_dict(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if evaluate:
+            return {self.visit(key, evaluate=True): self.visit(val)
+                    for key, val in obj.items()}
+        else:
+            return {self.visit(key, evaluate=False): self.visit(
+                val, evaluate=False) for key, val in obj.items()}
+
+    def v_list(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        return [self.visit(val, evaluate=evaluate) for val in obj]
+
+    v_str = v_obj
+    v_int = v_obj
+    v_float = v_obj
+    v_tuple = v_obj
+    v_complex = v_obj
+    v_bool = v_obj
+
+    def v_Array(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        _ar = []
+        for a in obj.children:
+            a = self.visit(a, evaluate=True)
+            if hasattr(a, "eval"):
+                a = a.eval
+            _ar.append(a)
+        obj.eval = _ar
+        return obj.eval if evaluate else obj
+
+    def v_Dict(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        _dict = {}
+        for cpl in obj.children:
+            cpl.left = self.visit(cpl.left, evaluate=True)
+            cpl.right = self.visit(cpl.right, evaluate=True)
+            cpl_left = cpl.left.eval \
+                if "eval" in dir(cpl.left) else cpl.left
+            cpl_right = cpl.right.eval \
+                if "eval" in dir(cpl.right) else cpl.right
+            _dict[cpl_left] = cpl_right
+        obj.eval = _dict
+        return obj.eval if evaluate else obj
+
+    def v_Func(self, obj, *args, **kwargs):
+        evaluate = kwargs["evaluate"]
+        if not hasattr(obj, "_id"):
+            obj._id = self.id()
+
+        for i, a in enumerate(obj.children):
+            a.eval = self.visit(a, evaluate=True)
+            obj.children[i] = a
+
+        fname = self.visit(obj.value, evaluate=True)
+
+        obj.call = getattr(Functions,
+                           fname, None)
+        if obj.call:
+            obj.eval = obj.call(self, *[a.eval for a in obj.children])
+        else:
+            return obj
+        return obj.eval if evaluate else obj
+
+
+class E3lmPlugin(E3lmInterpreter):
+    """Base class for an E3lm interpretation plugin.
+
+    `options` must contain a "key" that indicates what attribute to
+    assign to the program.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.options = kwargs
+        self.is_plugin = True
+
+    def interpret(self, input, source=None):
+        self.program = input
+        new_data = self.visit(self.program)
+        if "key" in self.options.keys():
+            attr = self.options["key"]
+        else:
+            raise NotImplementedError("Interpret is not implemented properly.")
+        setattr(self.program, attr, new_data)
+        return self.program
+
+    def v_Program(self, obj, *args, **kwargs):
+        for i, b in enumerate(obj.blocks):
+            b = self.visit(b)
+        return obj
+
+    def v_Block(self, obj, *args, **kwargs):
+        ast = False
+        if "ast" in self.options.keys():
+            ast = self.options["ast"]
+
+        for i, b in enumerate(obj.children):
+            b = self.visit(b)
+
+        for i, b in enumerate(obj.attrs):
+            b = self.visit(b)
+
+        return obj
```

### Comparing `e3lm-0.1.8/src/e3lm/lang/parser.py` & `e3lm-0.1.9/src/e3lm/lang/parser.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,425 +1,425 @@
-"""
-Author: Kenan Masri
-
-"""
-
-import os
-import re
-import textwrap
-from ply import yacc
-from e3lm.helpers.printers import _print, cprint
-from e3lm.utils.funcs import strip_once
-from e3lm.lang import ast
-from e3lm.lang.data import tokens, regexes
-from e3lm.lang.lexer import E3lmLexer
-
-
-class E3lmParser():
-    """The 3lm language parser."""
-    # --- Class variables ---
-    debug = False
-    tokens = tokens
-    scopes = [{
-        "last": None,
-        "next": None,
-        "current": None,
-    }]
-    print_method = _print
-    errors = []
-
-    # --- Rules ---
-    precedence = (
-        ('left', 'END',),
-        ('left', 'PLUS', 'MINUS'),
-        ('left', 'TIMES', 'DIVIDE'),
-    )
-
-    # Indefinite number of blocks under master
-    def p_master(self, p):
-        '''
-        master    : master block
-                  | block
-        '''
-        if len(p) == 3:
-            p[1].add(p[2])
-            p[0] = p[1]
-        else:
-            p[0] = ast.Program(imports=self.imports, blocks=[p[1]])
-
-    # Block variations
-    def p_block(self, p):
-        '''
-        block   : CLASS blockcontent END
-                | CLASS END
-        '''
-        if isinstance(p[1], tuple):
-            klass = p[1][0]
-            name = p[1][1]
-        else:
-            klass = p[1]
-            name = ""
-        bcontent = p[3] if len(p) == 5 \
-            else p[2] if len(p) == 4 and type(p[2]) == ast.BlockContent \
-            else None
-
-        b = ast.Block(klass, children=bcontent)
-        b.name = name
-        p[0] = b
-
-    # Block Content of other blocks and attrs
-    def p_blockcontent(self, p):
-        '''
-        blockcontent    : blockcontent attr
-                        | blockcontent block
-                        | attr
-                        | block
-        '''
-        if len(p) == 3:
-            p[0] = p[1]
-            p[0].children = p[1].children
-            if p[2].name not in [a.name for a in p[0].children
-                                 if type(a) == ast.Attr]:
-                p[0].children.extend([p[2]])
-            else:
-                self.errors.append([
-                    (AttributeError, p.lexpos(2),
-                     p.lexer.lexer.last_token.lineno-1),
-                    "Duplicate attribute '%s'" % p[2].name, p,
-                ])
-        else:
-            p[0] = ast.BlockContent([p[1]])
-
-    # Body and attrs
-    def p_attrset(self, p):
-        '''attr     : ATTR expr
-                    | BODY
-        '''
-        if len(p) > 2:
-            p[0] = ast.Attr(p[1], p[2])
-        else:
-            p[0] = ast.Attr("body", p[1],
-                            tokens=p.lexer.p_one.tokens or [])
-
-    # binary operations
-    def p_binops(self, p):
-        ''' expr    : expr PLUS term
-                    | expr MINUS term
-                    | term
-            term    : term TIMES factor
-                    | term DIVIDE factor
-                    | term TIMES TIMES factor
-                    | term DIVIDE DIVIDE factor
-                    | factor
-        '''
-        if len(p) == 2:
-            p[0] = p[1]
-        elif len(p) == 5:
-            if p[2] == "*" and p[3] == "*":
-                op = "**"
-            elif p[2] == "/" and p[3] == "/":
-                op = "//"
-            p[0] = ast.BinOp(op, p[1], p[4])
-        else:
-            p[0] = ast.BinOp(p[2], p[1], p[3])
-
-    # Number + unary as factors
-    def p_factor_num(self, p):
-        '''factor : NUM_INT
-                  | NUM_FLOAT
-                  | NUM_HEX
-                  | NUM_OCT
-                  | NUM_IMAG
-                  | NUM_BIN
-                  | PLUS factor
-                  | MINUS factor
-        '''
-        if p[1] in ("+", "-"):
-            p[0] = ast.UnaryOp(p[1], p[2])
-        else:
-            p[0] = ast.Num(p.lexer.p_one.value, p.lexer.p_one.type)
-
-    # parenthesis expr as factor
-    def p_factor_paren_expr(self, p):
-        '''factor : LPAREN expr RPAREN
-        '''
-        p[0] = p[2]
-
-    # Strings as factor
-    def p_factor_str(self, p):
-        '''factor : STRING
-        '''
-        p[0] = ast.Str(p[1])
-        p[0].type = p.lexer.p_one.quotes
-
-    def p_factor_bool(self, p):
-        '''factor : BOOL
-        '''
-        p[0] = ast.Bool(p[1])
-
-    def p_factor_none(self, p):
-        '''factor : NONE
-        '''
-        p[0] = ast.Undefined(p[1])
-
-    # Identifier as factor
-    def p_factor_id(self, p):
-        '''factor : identifier
-                  | func
-        '''
-        p[0] = p[1]
-
-    def p_func(self, p):
-        '''func   : ID LPAREN funcargs RPAREN
-                  | ID LPAREN RPAREN
-        '''
-        if len(p) == 5:
-            p[0] = ast.Func(p[1], p[3])
-        else:
-            p[0] = ast.Func(p[1], [])
-
-    def p_funcargs(self, p):
-        '''funcargs : funcargs COMMA expr
-                    | expr
-        '''
-        if len(p) == 4:
-            p[0] = p[1]
-            p[0].add(p[3])
-        else:
-            p[0] = ast.FuncArgs([p[1]])
-
-    def p_id_func(self, p):
-        '''identifier : factor DOT func
-                      | identifier DOT func
-        '''
-        p[0] = ast.Identifier([p[1], p[3]])
-
-    def p_id(self, p):
-        '''identifier : identifier DOT ID
-                      | factor DOT ID
-                      | func
-                      | ID
-        '''
-        if len(p) == 4:
-            if type(p[1]) == ast.Identifier:
-                p[0] = p[1]
-                p[0].add(p[3])
-            else:
-                p[0] = ast.Identifier([p[1], p[3]])
-        else:
-            p[0] = ast.Identifier([p[1]])
-
-    def p_id_index(self, p):
-        '''identifier : identifier LARRAY expr RARRAY
-        '''
-        p[0] = p[1]
-        p[0].add(ast.Index(p[3]))
-
-    # Arraydata additions
-    def p_arraydata(self, p):
-        '''arraydata : arraydata COMMA expr
-                     | expr
-        '''
-        if len(p) == 4:
-            p[0] = p[1]
-            p[0].add(p[3])
-        else:
-            p[0] = ast.Array([p[1], ])
-
-    # Basic array syntax
-    def p_factor_arr(self, p):
-        '''factor : LARRAY arraydata RARRAY
-                  | LARRAY arraydata COMMA RARRAY
-                  | LARRAY RARRAY
-        '''
-        if len(p) == 3:
-            p[0] = ast.Array([])
-        else:
-            p[0] = p[2]
-
-    # Dict additions
-    def p_dictdata(self, p):
-        '''dictdata : dictdata COMMA dictcouple
-                    | dictcouple
-        '''
-        if len(p) == 4:
-            p[0] = p[1]
-            p[0].add(p[3])
-        else:
-            p[0] = ast.DictData([p[1]])
-
-    def p_not(self, p):
-        '''expr : NOT expr
-        '''
-        p[0] = ast.UnaryOp('!', p[1])
-
-    def p_dict_dictdata(self, p):
-        '''dictdata : dict
-        '''
-        p[0] = p[1]
-
-    def p_factor_dictcouple(self, p):
-        '''dictcouple : expr COLON expr
-        '''
-        p[0] = ast.DictCouple(p[1], p[3])
-
-    def p_factor_dict(self, p):
-        '''dict   : LDICT dictdata RDICT
-                  | LDICT dictdata COMMA RDICT
-                  | LDICT RDICT
-        '''
-        p[0] = ast.Dict(p[2]) if len(p) != 3 else ast.Dict()
-
-    def p_dict(self, p):
-        '''factor : dict
-        '''
-        p[0] = p[1]
-
-    def p_error(self, p):
-        if p:
-            # curimport = self.srs
-            # for key,val in self.imports.items():
-            #     if val[0] <= p.lineno <= val[1]:
-            #         curimport = key
-
-            # lineno = p.lineno if curimport == self.srs \
-            #     else p.lineno - self.imports[curimport][0]
-
-            self.errors.append([
-                (SyntaxError, p.lexpos, p.lineno), "Syntax error near token "
-                + str(p), p,
-            ])
-            # self.parser.errok()
-        else:
-            self.print_method("Syntax error at EOF", "ERROR")
-
-    # --- Functions ---
-    # -- Class functions
-
-    def build(self, **kwargs):
-        if 'debug' in kwargs.keys():
-            self.debug = kwargs.pop('debug')
-        self.print_method = _print
-        if 'enable_colors' in kwargs.keys():
-            if kwargs.pop('enable_colors') == True:
-                self.print_method = cprint
-        if 'lexer' in kwargs.keys():
-            self.e3lmLexer = kwargs.pop('lexer')
-        else:
-            self.e3lmLexer = E3lmLexer()
-            if 'lexer_kwargs' in kwargs.keys():
-                lwargs = kwargs['lexer_kwargs']
-            else:
-                lwargs = {}
-            self.e3lmLexer.build(**lwargs)
-        self.tokens = self.e3lmLexer.tokens
-        if 'yacc_kwargs' not in kwargs.keys():
-            kwargs['yacc_kwargs'] = {}
-        self.parser = yacc.yacc(module=self, debug=(self.debug >= 2),
-                                **kwargs['yacc_kwargs']
-                                )
-        self.parser.e3lm_parser = self
-        self.parser.last_node = None
-        if 'tracking' in kwargs['yacc_kwargs'].keys():
-            self.tracking = kwargs['yacc_kwargs']['tracking']
-        else:
-            if 'tracking' in kwargs.keys():
-                self.tracking = kwargs['tracking']
-            else:
-                self.tracking = False
-        self.errors = []
-
-    def parse(self, input, source=None, **kwargs):
-        # get curpath for imports
-        is_file = False
-
-        if input.count("\n") == 0 and os.path.exists(input):
-            is_file = True
-            self.srs = os.path.abspath(input)
-            self.curpath = self.srs
-            source = input
-
-        self.srs = "<string>"
-        if source:
-            if os.path.exists(source):
-                self.srs = os.path.abspath(source)
-                self.curpath = self.srs
-
-        if not is_file:
-            textinput = input
-            self.curpath = os.getcwd()
-        else:
-            self.curpath = os.path.dirname(os.path.abspath(input))
-            with open(self.srs, 'r', encoding='utf-8') as f:
-                textinput = "".join(f.readlines())
-
-        # Before parsing-and-lexing filters
-        textinput = self.do_imports(textinput)
-        result = self.parser.parse(textinput, self.e3lmLexer, **kwargs)
-
-        if self.debug >= 1:
-            if len(self.errors) > 0:
-                for err in self.errors:
-                    if ('tracking' in kwargs.keys() and kwargs['tracking']) \
-                            or self.tracking:
-                        self.print_method((err[0], err[1]), "ERROR")
-                    else:
-                        self.print_method((err[1]), "ERROR")
-        return result
-
-    def do_imports(self, text):
-        """Regex the import statements from `input` and load them."""
-        curpath = os.path.dirname(self.srs)
-
-        def get_file(fname):
-            """Check for `fname` existence relative to main file dir (or
-            cwd)."""
-            fname = strip_once(fname, "\"\'")
-            filename, fileext = os.path.splitext(fname)
-            if not fileext:
-                fname = fname + ".3lm"
-            fpath = curpath + os.path.sep + fname
-            if not os.path.exists(fpath):
-                fpath = os.path.abspath(fname)
-                if not os.path.exists(fpath):
-                    raise Exception("'{}' does not exist.".format(fpath))
-            return fpath
-
-        regex = regexes["IMPORT"]
-        data = text.splitlines(True)
-        self.imports = {}
-        curimport = self.srs
-        _lastcurimport = self.srs
-        linecounter = {self.srs: 0, }
-        for lineno, line in enumerate(data):
-            curimport = self.srs
-            for key, val in self.imports.items():
-                if val[0] <= lineno <= val[1]:
-                    curimport = key
-
-            if _lastcurimport != curimport:
-                _lastcurimport = curimport
-                linecounter[curimport] = 0
-
-            linecounter[curimport] += 1
-            match = re.match(regex, line)
-            if match:
-                m = match.group(3)
-                fpath = get_file(m)
-                if fpath in self.imports.keys():
-                    raise SyntaxError(
-                        "Importing '{}' again.".format(
-                            os.path.basename(fpath)
-                        ),
-                        (curimport,
-                            linecounter[curimport]+1, match.end(1), line
-                         )
-                    )
-                with open(fpath, "r", encoding='utf-8') as f:
-                    new = f.readlines()
-                new.append("\n")
-                self.imports[fpath] = (lineno+1, lineno+len(new))
-                data[lineno] = ""
-                for i, l in enumerate(new):
-                    data.insert(lineno+i, l)
-
-        return "".join(data)
+"""
+Author: Kenan Masri
+
+"""
+
+import os
+import re
+import textwrap
+from ply import yacc
+from e3lm.helpers.printers import _print, cprint
+from e3lm.utils.funcs import strip_once
+from e3lm.lang import ast
+from e3lm.lang.data import tokens, regexes
+from e3lm.lang.lexer import E3lmLexer
+
+
+class E3lmParser():
+    """The 3lm language parser."""
+    # --- Class variables ---
+    debug = False
+    tokens = tokens
+    scopes = [{
+        "last": None,
+        "next": None,
+        "current": None,
+    }]
+    print_method = _print
+    errors = []
+
+    # --- Rules ---
+    precedence = (
+        ('left', 'END',),
+        ('left', 'PLUS', 'MINUS'),
+        ('left', 'TIMES', 'DIVIDE'),
+    )
+
+    # Indefinite number of blocks under master
+    def p_master(self, p):
+        '''
+        master    : master block
+                  | block
+        '''
+        if len(p) == 3:
+            p[1].add(p[2])
+            p[0] = p[1]
+        else:
+            p[0] = ast.Program(imports=self.imports, blocks=[p[1]])
+
+    # Block variations
+    def p_block(self, p):
+        '''
+        block   : CLASS blockcontent END
+                | CLASS END
+        '''
+        if isinstance(p[1], tuple):
+            klass = p[1][0]
+            name = p[1][1]
+        else:
+            klass = p[1]
+            name = ""
+        bcontent = p[3] if len(p) == 5 \
+            else p[2] if len(p) == 4 and type(p[2]) == ast.BlockContent \
+            else None
+
+        b = ast.Block(klass, children=bcontent)
+        b.name = name
+        p[0] = b
+
+    # Block Content of other blocks and attrs
+    def p_blockcontent(self, p):
+        '''
+        blockcontent    : blockcontent attr
+                        | blockcontent block
+                        | attr
+                        | block
+        '''
+        if len(p) == 3:
+            p[0] = p[1]
+            p[0].children = p[1].children
+            if p[2].name not in [a.name for a in p[0].children
+                                 if type(a) == ast.Attr]:
+                p[0].children.extend([p[2]])
+            else:
+                self.errors.append([
+                    (AttributeError, p.lexpos(2),
+                     p.lexer.lexer.last_token.lineno-1),
+                    "Duplicate attribute '%s'" % p[2].name, p,
+                ])
+        else:
+            p[0] = ast.BlockContent([p[1]])
+
+    # Body and attrs
+    def p_attrset(self, p):
+        '''attr     : ATTR expr
+                    | BODY
+        '''
+        if len(p) > 2:
+            p[0] = ast.Attr(p[1], p[2])
+        else:
+            p[0] = ast.Attr("body", p[1],
+                            tokens=p.lexer.p_one.tokens or [])
+
+    # binary operations
+    def p_binops(self, p):
+        ''' expr    : expr PLUS term
+                    | expr MINUS term
+                    | term
+            term    : term TIMES factor
+                    | term DIVIDE factor
+                    | term TIMES TIMES factor
+                    | term DIVIDE DIVIDE factor
+                    | factor
+        '''
+        if len(p) == 2:
+            p[0] = p[1]
+        elif len(p) == 5:
+            if p[2] == "*" and p[3] == "*":
+                op = "**"
+            elif p[2] == "/" and p[3] == "/":
+                op = "//"
+            p[0] = ast.BinOp(op, p[1], p[4])
+        else:
+            p[0] = ast.BinOp(p[2], p[1], p[3])
+
+    # Number + unary as factors
+    def p_factor_num(self, p):
+        '''factor : NUM_INT
+                  | NUM_FLOAT
+                  | NUM_HEX
+                  | NUM_OCT
+                  | NUM_IMAG
+                  | NUM_BIN
+                  | PLUS factor
+                  | MINUS factor
+        '''
+        if p[1] in ("+", "-"):
+            p[0] = ast.UnaryOp(p[1], p[2])
+        else:
+            p[0] = ast.Num(p.lexer.p_one.value, p.lexer.p_one.type)
+
+    # parenthesis expr as factor
+    def p_factor_paren_expr(self, p):
+        '''factor : LPAREN expr RPAREN
+        '''
+        p[0] = p[2]
+
+    # Strings as factor
+    def p_factor_str(self, p):
+        '''factor : STRING
+        '''
+        p[0] = ast.Str(p[1])
+        p[0].type = p.lexer.p_one.quotes
+
+    def p_factor_bool(self, p):
+        '''factor : BOOL
+        '''
+        p[0] = ast.Bool(p[1])
+
+    def p_factor_none(self, p):
+        '''factor : NONE
+        '''
+        p[0] = ast.Undefined(p[1])
+
+    # Identifier as factor
+    def p_factor_id(self, p):
+        '''factor : identifier
+                  | func
+        '''
+        p[0] = p[1]
+
+    def p_func(self, p):
+        '''func   : ID LPAREN funcargs RPAREN
+                  | ID LPAREN RPAREN
+        '''
+        if len(p) == 5:
+            p[0] = ast.Func(p[1], p[3])
+        else:
+            p[0] = ast.Func(p[1], [])
+
+    def p_funcargs(self, p):
+        '''funcargs : funcargs COMMA expr
+                    | expr
+        '''
+        if len(p) == 4:
+            p[0] = p[1]
+            p[0].add(p[3])
+        else:
+            p[0] = ast.FuncArgs([p[1]])
+
+    def p_id_func(self, p):
+        '''identifier : factor DOT func
+                      | identifier DOT func
+        '''
+        p[0] = ast.Identifier([p[1], p[3]])
+
+    def p_id(self, p):
+        '''identifier : identifier DOT ID
+                      | factor DOT ID
+                      | func
+                      | ID
+        '''
+        if len(p) == 4:
+            if type(p[1]) == ast.Identifier:
+                p[0] = p[1]
+                p[0].add(p[3])
+            else:
+                p[0] = ast.Identifier([p[1], p[3]])
+        else:
+            p[0] = ast.Identifier([p[1]])
+
+    def p_id_index(self, p):
+        '''identifier : identifier LARRAY expr RARRAY
+        '''
+        p[0] = p[1]
+        p[0].add(ast.Index(p[3]))
+
+    # Arraydata additions
+    def p_arraydata(self, p):
+        '''arraydata : arraydata COMMA expr
+                     | expr
+        '''
+        if len(p) == 4:
+            p[0] = p[1]
+            p[0].add(p[3])
+        else:
+            p[0] = ast.Array([p[1], ])
+
+    # Basic array syntax
+    def p_factor_arr(self, p):
+        '''factor : LARRAY arraydata RARRAY
+                  | LARRAY arraydata COMMA RARRAY
+                  | LARRAY RARRAY
+        '''
+        if len(p) == 3:
+            p[0] = ast.Array([])
+        else:
+            p[0] = p[2]
+
+    # Dict additions
+    def p_dictdata(self, p):
+        '''dictdata : dictdata COMMA dictcouple
+                    | dictcouple
+        '''
+        if len(p) == 4:
+            p[0] = p[1]
+            p[0].add(p[3])
+        else:
+            p[0] = ast.DictData([p[1]])
+
+    def p_not(self, p):
+        '''expr : NOT expr
+        '''
+        p[0] = ast.UnaryOp('!', p[1])
+
+    def p_dict_dictdata(self, p):
+        '''dictdata : dict
+        '''
+        p[0] = p[1]
+
+    def p_factor_dictcouple(self, p):
+        '''dictcouple : expr COLON expr
+        '''
+        p[0] = ast.DictCouple(p[1], p[3])
+
+    def p_factor_dict(self, p):
+        '''dict   : LDICT dictdata RDICT
+                  | LDICT dictdata COMMA RDICT
+                  | LDICT RDICT
+        '''
+        p[0] = ast.Dict(p[2]) if len(p) != 3 else ast.Dict()
+
+    def p_dict(self, p):
+        '''factor : dict
+        '''
+        p[0] = p[1]
+
+    def p_error(self, p):
+        if p:
+            # curimport = self.srs
+            # for key,val in self.imports.items():
+            #     if val[0] <= p.lineno <= val[1]:
+            #         curimport = key
+
+            # lineno = p.lineno if curimport == self.srs \
+            #     else p.lineno - self.imports[curimport][0]
+
+            self.errors.append([
+                (SyntaxError, p.lexpos, p.lineno), "Syntax error near token "
+                + str(p), p,
+            ])
+            # self.parser.errok()
+        else:
+            self.print_method("Syntax error at EOF", "ERROR")
+
+    # --- Functions ---
+    # -- Class functions
+
+    def build(self, **kwargs):
+        if 'debug' in kwargs.keys():
+            self.debug = kwargs.pop('debug')
+        self.print_method = _print
+        if 'enable_colors' in kwargs.keys():
+            if kwargs.pop('enable_colors') == True:
+                self.print_method = cprint
+        if 'lexer' in kwargs.keys():
+            self.e3lmLexer = kwargs.pop('lexer')
+        else:
+            self.e3lmLexer = E3lmLexer()
+            if 'lexer_kwargs' in kwargs.keys():
+                lwargs = kwargs['lexer_kwargs']
+            else:
+                lwargs = {}
+            self.e3lmLexer.build(**lwargs)
+        self.tokens = self.e3lmLexer.tokens
+        if 'yacc_kwargs' not in kwargs.keys():
+            kwargs['yacc_kwargs'] = {}
+        self.parser = yacc.yacc(module=self, debug=(self.debug >= 2),
+                                **kwargs['yacc_kwargs']
+                                )
+        self.parser.e3lm_parser = self
+        self.parser.last_node = None
+        if 'tracking' in kwargs['yacc_kwargs'].keys():
+            self.tracking = kwargs['yacc_kwargs']['tracking']
+        else:
+            if 'tracking' in kwargs.keys():
+                self.tracking = kwargs['tracking']
+            else:
+                self.tracking = False
+        self.errors = []
+
+    def parse(self, input, source=None, **kwargs):
+        # get curpath for imports
+        is_file = False
+
+        if input.count("\n") == 0 and os.path.exists(input):
+            is_file = True
+            self.srs = os.path.abspath(input)
+            self.curpath = self.srs
+            source = input
+
+        self.srs = "<string>"
+        if source:
+            if os.path.exists(source):
+                self.srs = os.path.abspath(source)
+                self.curpath = self.srs
+
+        if not is_file:
+            textinput = input
+            self.curpath = os.getcwd()
+        else:
+            self.curpath = os.path.dirname(os.path.abspath(input))
+            with open(self.srs, 'r', encoding='utf-8') as f:
+                textinput = "".join(f.readlines())
+
+        # Before parsing-and-lexing filters
+        textinput = self.do_imports(textinput)
+        result = self.parser.parse(textinput, self.e3lmLexer, **kwargs)
+
+        if self.debug >= 1:
+            if len(self.errors) > 0:
+                for err in self.errors:
+                    if ('tracking' in kwargs.keys() and kwargs['tracking']) \
+                            or self.tracking:
+                        self.print_method((err[0], err[1]), "ERROR")
+                    else:
+                        self.print_method((err[1]), "ERROR")
+        return result
+
+    def do_imports(self, text):
+        """Regex the import statements from `input` and load them."""
+        curpath = os.path.dirname(self.srs)
+
+        def get_file(fname):
+            """Check for `fname` existence relative to main file dir (or
+            cwd)."""
+            fname = strip_once(fname, "\"\'")
+            filename, fileext = os.path.splitext(fname)
+            if not fileext:
+                fname = fname + ".3lm"
+            fpath = curpath + os.path.sep + fname
+            if not os.path.exists(fpath):
+                fpath = os.path.abspath(fname)
+                if not os.path.exists(fpath):
+                    raise Exception("'{}' does not exist.".format(fpath))
+            return fpath
+
+        regex = regexes["IMPORT"]
+        data = text.splitlines(True)
+        self.imports = {}
+        curimport = self.srs
+        _lastcurimport = self.srs
+        linecounter = {self.srs: 0, }
+        for lineno, line in enumerate(data):
+            curimport = self.srs
+            for key, val in self.imports.items():
+                if val[0] <= lineno <= val[1]:
+                    curimport = key
+
+            if _lastcurimport != curimport:
+                _lastcurimport = curimport
+                linecounter[curimport] = 0
+
+            linecounter[curimport] += 1
+            match = re.match(regex, line)
+            if match:
+                m = match.group(3)
+                fpath = get_file(m)
+                if fpath in self.imports.keys():
+                    raise SyntaxError(
+                        "Importing '{}' again.".format(
+                            os.path.basename(fpath)
+                        ),
+                        (curimport,
+                            linecounter[curimport]+1, match.end(1), line
+                         )
+                    )
+                with open(fpath, "r", encoding='utf-8') as f:
+                    new = f.readlines()
+                new.append("\n")
+                self.imports[fpath] = (lineno+1, lineno+len(new))
+                data[lineno] = ""
+                for i, l in enumerate(new):
+                    data.insert(lineno+i, l)
+
+        return "".join(data)
```

### Comparing `e3lm-0.1.8/src/e3lm/lang/parsetab.py` & `e3lm-0.1.9/src/e3lm/lang/parsetab.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-
-# parsetab.py
-# This file is automatically generated. Do not edit.
-# pylint: disable=W,C,R
-_tabversion = '3.10'
-
-_lr_method = 'LALR'
-
-_lr_signature = 'leftENDleftPLUSMINUSleftTIMESDIVIDEAND ATTR AVAL BODY BOOL CLASS COLON COMMA COMMENT DIVIDE DOT END ID IMPORT LARRAY LDICT LPAREN MINUS NAME NEWLINE NONE NOT NUM_BIN NUM_FLOAT NUM_HEX NUM_IMAG NUM_INT NUM_OCT OR PLUS RARRAY RDICT RPAREN STRING STRING_CONTINUE STRING_CONTINUE_NEWLINE STRING_END STRING_START_SINGLEQ1 STRING_START_SINGLEQ2 STRING_START_TRIPLEQ1 STRING_START_TRIPLEQ2 TERM TIMES UNIT WS\n        master    : master block\n                  | block\n        \n        block   : CLASS blockcontent END\n                | CLASS END\n        \n        blockcontent    : blockcontent attr\n                        | blockcontent block\n                        | attr\n                        | block\n        attr     : ATTR expr\n                    | BODY\n         expr    : expr PLUS term\n                    | expr MINUS term\n                    | term\n            term    : term TIMES factor\n                    | term DIVIDE factor\n                    | term TIMES TIMES factor\n                    | term DIVIDE DIVIDE factor\n                    | factor\n        factor : NUM_INT\n                  | NUM_FLOAT\n                  | NUM_HEX\n                  | NUM_OCT\n                  | NUM_IMAG\n                  | NUM_BIN\n                  | PLUS factor\n                  | MINUS factor\n        factor : LPAREN expr RPAREN\n        factor : STRING\n        factor : BOOL\n        factor : NONE\n        factor : identifier\n                  | func\n        func   : ID LPAREN funcargs RPAREN\n                  | ID LPAREN RPAREN\n        funcargs : funcargs COMMA expr\n                    | expr\n        identifier : factor DOT func\n                      | identifier DOT func\n        identifier : identifier DOT ID\n                      | factor DOT ID\n                      | func\n                      | ID\n        identifier : identifier LARRAY expr RARRAY\n        arraydata : arraydata COMMA expr\n                     | expr\n        factor : LARRAY arraydata RARRAY\n                  | LARRAY arraydata COMMA RARRAY\n                  | LARRAY RARRAY\n        dictdata : dictdata COMMA dictcouple\n                    | dictcouple\n        expr : NOT expr\n        dictdata : dict\n        dictcouple : expr COLON expr\n        dict   : LDICT dictdata RDICT\n                  | LDICT dictdata COMMA RDICT\n                  | LDICT RDICT\n        factor : dict\n        '
-    
-_lr_action_items = {'CLASS':([0,1,2,3,4,5,6,7,8,10,11,12,13,14,16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,48,52,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[3,3,-2,3,-1,3,-4,-7,-8,-10,-3,-5,-6,-9,-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,-48,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'$end':([1,2,4,6,11,],[0,-2,-1,-4,-3,]),'END':([3,5,6,7,8,10,11,12,13,14,16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,48,52,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[6,11,-4,-7,-8,-10,-3,-5,-6,-9,-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,-48,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'ATTR':([3,5,6,7,8,10,11,12,13,14,16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,48,52,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[9,9,-4,-7,-8,-10,-3,-5,-6,-9,-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,-48,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'BODY':([3,5,6,7,8,10,11,12,13,14,16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,48,52,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[10,10,-4,-7,-8,-10,-3,-5,-6,-9,-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,-48,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'NOT':([9,18,26,32,35,46,50,69,74,75,82,],[18,18,18,18,18,18,18,18,18,18,18,]),'NUM_INT':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,]),'NUM_FLOAT':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,]),'NUM_HEX':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,]),'NUM_OCT':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[23,23,23,23,23,23,23,23,23,23,23,23,23,23,23,23,23,23,23,]),'NUM_IMAG':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[24,24,24,24,24,24,24,24,24,24,24,24,24,24,24,24,24,24,24,]),'NUM_BIN':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,]),'PLUS':([9,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,44,46,48,49,50,52,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,71,72,73,74,75,76,77,78,79,80,81,82,83,85,86,],[15,36,15,-13,15,15,-18,-19,-20,-21,-22,-23,-24,15,-28,-29,-30,-31,-32,15,-57,-42,15,15,15,-25,15,15,-26,36,36,15,-48,36,15,-56,-57,36,-11,-12,15,-14,15,-15,-37,-40,-27,-38,-39,36,-46,15,-34,36,-54,15,15,-16,-17,-43,-47,36,-33,15,-55,36,36,]),'MINUS':([9,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,44,46,48,49,50,52,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,71,72,73,74,75,76,77,78,79,80,81,82,83,85,86,],[17,37,17,-13,17,17,-18,-19,-20,-21,-22,-23,-24,17,-28,-29,-30,-31,-32,17,-57,-42,17,17,17,-25,17,17,-26,37,37,17,-48,37,17,-56,-57,37,-11,-12,17,-14,17,-15,-37,-40,-27,-38,-39,37,-46,17,-34,37,-54,17,17,-16,-17,-43,-47,37,-33,17,-55,37,37,]),'LPAREN':([9,15,17,18,26,32,34,35,36,37,39,40,46,50,58,60,63,66,69,74,75,82,],[26,26,26,26,26,26,50,26,26,26,26,26,26,26,26,26,50,50,26,26,26,26,]),'STRING':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,]),'BOOL':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,]),'NONE':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,]),'LARRAY':([9,15,17,18,26,30,31,32,34,35,36,37,39,40,46,50,58,60,62,63,65,66,69,71,74,75,78,81,82,],[32,32,32,32,32,46,-41,32,-42,32,32,32,32,32,32,32,32,32,-37,-40,-38,-39,32,-34,32,32,-43,-33,32,]),'ID':([9,15,17,18,26,32,35,36,37,39,40,43,45,46,50,58,60,69,74,75,82,],[34,34,34,34,34,34,34,34,34,34,34,63,66,34,34,34,34,34,34,34,34,]),'LDICT':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[35,35,35,35,35,35,35,35,35,35,35,35,35,35,35,35,35,35,35,]),'RPAREN':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,44,48,50,52,56,57,59,61,62,63,64,65,66,68,70,71,72,73,76,77,78,79,81,83,86,],[-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,64,-48,71,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,81,-34,-36,-54,-16,-17,-43,-47,-33,-55,-35,]),'RARRAY':([16,19,20,21,22,23,24,25,27,28,29,30,31,32,33,34,38,41,42,47,48,49,52,56,57,59,61,62,63,64,65,66,67,68,69,71,73,76,77,78,79,80,81,83,],[-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,48,-57,-42,-25,-26,-51,68,-48,-45,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,78,-46,79,-34,-54,-16,-17,-43,-47,-44,-33,-55,]),'COMMA':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,47,48,49,51,52,53,54,56,57,59,61,62,63,64,65,66,68,70,71,72,73,76,77,78,79,80,81,83,84,85,86,],[-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,69,-48,-45,74,-56,-50,-52,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,82,-34,-36,-54,-16,-17,-43,-47,-44,-33,-55,-49,-53,-35,]),'COLON':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,48,52,54,55,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,-48,-56,-57,75,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'RDICT':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,35,38,41,42,48,51,52,53,54,56,57,59,61,62,63,64,65,66,68,71,73,74,76,77,78,79,81,83,84,85,],[-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,52,-25,-26,-51,-48,73,-56,-50,-52,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,83,-16,-17,-43,-47,-33,-55,-49,-53,]),'TIMES':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,39,41,48,52,54,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[39,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,58,-26,-48,-56,-57,39,39,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'DIVIDE':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,40,41,48,52,54,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[40,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,60,-26,-48,-56,-57,40,40,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'DOT':([19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,48,52,54,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[43,-19,-20,-21,-22,-23,-24,-28,-29,-30,45,-32,-57,-42,-25,-26,-48,-56,-57,43,43,-37,-40,-27,-38,-39,-46,-34,-54,43,43,-43,-47,-33,-55,]),}
-
-_lr_action = {}
-for _k, _v in _lr_action_items.items():
-   for _x,_y in zip(_v[0],_v[1]):
-      if not _x in _lr_action:  _lr_action[_x] = {}
-      _lr_action[_x][_k] = _y
-del _lr_action_items
-
-_lr_goto_items = {'master':([0,],[1,]),'block':([0,1,3,5,],[2,4,8,13,]),'blockcontent':([3,],[5,]),'attr':([3,5,],[7,12,]),'expr':([9,18,26,32,35,46,50,69,74,75,82,],[14,42,44,49,55,67,72,80,55,85,86,]),'term':([9,18,26,32,35,36,37,46,50,69,74,75,82,],[16,16,16,16,16,56,57,16,16,16,16,16,16,]),'factor':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[19,38,41,19,19,19,19,19,19,59,61,19,19,76,77,19,19,19,19,]),'identifier':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,]),'func':([9,15,17,18,26,32,35,36,37,39,40,43,45,46,50,58,60,69,74,75,82,],[31,31,31,31,31,31,31,31,31,31,31,62,65,31,31,31,31,31,31,31,31,]),'dict':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[33,33,33,33,33,33,54,33,33,33,33,33,33,33,33,33,33,33,33,]),'arraydata':([32,],[47,]),'dictdata':([35,],[51,]),'dictcouple':([35,74,],[53,84,]),'funcargs':([50,],[70,]),}
-
-_lr_goto = {}
-for _k, _v in _lr_goto_items.items():
-   for _x, _y in zip(_v[0], _v[1]):
-       if not _x in _lr_goto: _lr_goto[_x] = {}
-       _lr_goto[_x][_k] = _y
-del _lr_goto_items
-_lr_productions = [
-  ("S' -> master","S'",1,None,None,None),
-  ('master -> master block','master',2,'p_master','parser.py',40),
-  ('master -> block','master',1,'p_master','parser.py',41),
-  ('block -> CLASS blockcontent END','block',3,'p_block','parser.py',52),
-  ('block -> CLASS END','block',2,'p_block','parser.py',53),
-  ('blockcontent -> blockcontent attr','blockcontent',2,'p_blockcontent','parser.py',70),
-  ('blockcontent -> blockcontent block','blockcontent',2,'p_blockcontent','parser.py',71),
-  ('blockcontent -> attr','blockcontent',1,'p_blockcontent','parser.py',72),
-  ('blockcontent -> block','blockcontent',1,'p_blockcontent','parser.py',73),
-  ('attr -> ATTR expr','attr',2,'p_attrset','parser.py',91),
-  ('attr -> BODY','attr',1,'p_attrset','parser.py',92),
-  ('expr -> expr PLUS term','expr',3,'p_binops','parser.py',102),
-  ('expr -> expr MINUS term','expr',3,'p_binops','parser.py',103),
-  ('expr -> term','expr',1,'p_binops','parser.py',104),
-  ('term -> term TIMES factor','term',3,'p_binops','parser.py',105),
-  ('term -> term DIVIDE factor','term',3,'p_binops','parser.py',106),
-  ('term -> term TIMES TIMES factor','term',4,'p_binops','parser.py',107),
-  ('term -> term DIVIDE DIVIDE factor','term',4,'p_binops','parser.py',108),
-  ('term -> factor','term',1,'p_binops','parser.py',109),
-  ('factor -> NUM_INT','factor',1,'p_factor_num','parser.py',124),
-  ('factor -> NUM_FLOAT','factor',1,'p_factor_num','parser.py',125),
-  ('factor -> NUM_HEX','factor',1,'p_factor_num','parser.py',126),
-  ('factor -> NUM_OCT','factor',1,'p_factor_num','parser.py',127),
-  ('factor -> NUM_IMAG','factor',1,'p_factor_num','parser.py',128),
-  ('factor -> NUM_BIN','factor',1,'p_factor_num','parser.py',129),
-  ('factor -> PLUS factor','factor',2,'p_factor_num','parser.py',130),
-  ('factor -> MINUS factor','factor',2,'p_factor_num','parser.py',131),
-  ('factor -> LPAREN expr RPAREN','factor',3,'p_factor_paren_expr','parser.py',140),
-  ('factor -> STRING','factor',1,'p_factor_str','parser.py',146),
-  ('factor -> BOOL','factor',1,'p_factor_bool','parser.py',152),
-  ('factor -> NONE','factor',1,'p_factor_none','parser.py',157),
-  ('factor -> identifier','factor',1,'p_factor_id','parser.py',163),
-  ('factor -> func','factor',1,'p_factor_id','parser.py',164),
-  ('func -> ID LPAREN funcargs RPAREN','func',4,'p_func','parser.py',169),
-  ('func -> ID LPAREN RPAREN','func',3,'p_func','parser.py',170),
-  ('funcargs -> funcargs COMMA expr','funcargs',3,'p_funcargs','parser.py',178),
-  ('funcargs -> expr','funcargs',1,'p_funcargs','parser.py',179),
-  ('identifier -> factor DOT func','identifier',3,'p_id_func','parser.py',188),
-  ('identifier -> identifier DOT func','identifier',3,'p_id_func','parser.py',189),
-  ('identifier -> identifier DOT ID','identifier',3,'p_id','parser.py',194),
-  ('identifier -> factor DOT ID','identifier',3,'p_id','parser.py',195),
-  ('identifier -> func','identifier',1,'p_id','parser.py',196),
-  ('identifier -> ID','identifier',1,'p_id','parser.py',197),
-  ('identifier -> identifier LARRAY expr RARRAY','identifier',4,'p_id_index','parser.py',209),
-  ('arraydata -> arraydata COMMA expr','arraydata',3,'p_arraydata','parser.py',216),
-  ('arraydata -> expr','arraydata',1,'p_arraydata','parser.py',217),
-  ('factor -> LARRAY arraydata RARRAY','factor',3,'p_factor_arr','parser.py',227),
-  ('factor -> LARRAY arraydata COMMA RARRAY','factor',4,'p_factor_arr','parser.py',228),
-  ('factor -> LARRAY RARRAY','factor',2,'p_factor_arr','parser.py',229),
-  ('dictdata -> dictdata COMMA dictcouple','dictdata',3,'p_dictdata','parser.py',238),
-  ('dictdata -> dictcouple','dictdata',1,'p_dictdata','parser.py',239),
-  ('expr -> NOT expr','expr',2,'p_not','parser.py',248),
-  ('dictdata -> dict','dictdata',1,'p_dict_dictdata','parser.py',253),
-  ('dictcouple -> expr COLON expr','dictcouple',3,'p_factor_dictcouple','parser.py',258),
-  ('dict -> LDICT dictdata RDICT','dict',3,'p_factor_dict','parser.py',263),
-  ('dict -> LDICT dictdata COMMA RDICT','dict',4,'p_factor_dict','parser.py',264),
-  ('dict -> LDICT RDICT','dict',2,'p_factor_dict','parser.py',265),
-  ('factor -> dict','factor',1,'p_dict','parser.py',270),
-]
+
+# parsetab.py
+# This file is automatically generated. Do not edit.
+# pylint: disable=W,C,R
+_tabversion = '3.10'
+
+_lr_method = 'LALR'
+
+_lr_signature = 'leftENDleftPLUSMINUSleftTIMESDIVIDEAND ATTR AVAL BODY BOOL CLASS COLON COMMA COMMENT DIVIDE DOT END ID IMPORT LARRAY LDICT LPAREN MINUS NAME NEWLINE NONE NOT NUM_BIN NUM_FLOAT NUM_HEX NUM_IMAG NUM_INT NUM_OCT OR PLUS RARRAY RDICT RPAREN STRING STRING_CONTINUE STRING_CONTINUE_NEWLINE STRING_END STRING_START_SINGLEQ1 STRING_START_SINGLEQ2 STRING_START_TRIPLEQ1 STRING_START_TRIPLEQ2 TERM TIMES UNIT WS\n        master    : master block\n                  | block\n        \n        block   : CLASS blockcontent END\n                | CLASS END\n        \n        blockcontent    : blockcontent attr\n                        | blockcontent block\n                        | attr\n                        | block\n        attr     : ATTR expr\n                    | BODY\n         expr    : expr PLUS term\n                    | expr MINUS term\n                    | term\n            term    : term TIMES factor\n                    | term DIVIDE factor\n                    | term TIMES TIMES factor\n                    | term DIVIDE DIVIDE factor\n                    | factor\n        factor : NUM_INT\n                  | NUM_FLOAT\n                  | NUM_HEX\n                  | NUM_OCT\n                  | NUM_IMAG\n                  | NUM_BIN\n                  | PLUS factor\n                  | MINUS factor\n        factor : LPAREN expr RPAREN\n        factor : STRING\n        factor : BOOL\n        factor : NONE\n        factor : identifier\n                  | func\n        func   : ID LPAREN funcargs RPAREN\n                  | ID LPAREN RPAREN\n        funcargs : funcargs COMMA expr\n                    | expr\n        identifier : factor DOT func\n                      | identifier DOT func\n        identifier : identifier DOT ID\n                      | factor DOT ID\n                      | func\n                      | ID\n        identifier : identifier LARRAY expr RARRAY\n        arraydata : arraydata COMMA expr\n                     | expr\n        factor : LARRAY arraydata RARRAY\n                  | LARRAY arraydata COMMA RARRAY\n                  | LARRAY RARRAY\n        dictdata : dictdata COMMA dictcouple\n                    | dictcouple\n        expr : NOT expr\n        dictdata : dict\n        dictcouple : expr COLON expr\n        dict   : LDICT dictdata RDICT\n                  | LDICT dictdata COMMA RDICT\n                  | LDICT RDICT\n        factor : dict\n        '
+    
+_lr_action_items = {'CLASS':([0,1,2,3,4,5,6,7,8,10,11,12,13,14,16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,48,52,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[3,3,-2,3,-1,3,-4,-7,-8,-10,-3,-5,-6,-9,-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,-48,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'$end':([1,2,4,6,11,],[0,-2,-1,-4,-3,]),'END':([3,5,6,7,8,10,11,12,13,14,16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,48,52,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[6,11,-4,-7,-8,-10,-3,-5,-6,-9,-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,-48,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'ATTR':([3,5,6,7,8,10,11,12,13,14,16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,48,52,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[9,9,-4,-7,-8,-10,-3,-5,-6,-9,-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,-48,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'BODY':([3,5,6,7,8,10,11,12,13,14,16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,48,52,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[10,10,-4,-7,-8,-10,-3,-5,-6,-9,-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,-48,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'NOT':([9,18,26,32,35,46,50,69,74,75,82,],[18,18,18,18,18,18,18,18,18,18,18,]),'NUM_INT':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,]),'NUM_FLOAT':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,]),'NUM_HEX':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,]),'NUM_OCT':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[23,23,23,23,23,23,23,23,23,23,23,23,23,23,23,23,23,23,23,]),'NUM_IMAG':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[24,24,24,24,24,24,24,24,24,24,24,24,24,24,24,24,24,24,24,]),'NUM_BIN':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,25,]),'PLUS':([9,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,44,46,48,49,50,52,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,71,72,73,74,75,76,77,78,79,80,81,82,83,85,86,],[15,36,15,-13,15,15,-18,-19,-20,-21,-22,-23,-24,15,-28,-29,-30,-31,-32,15,-57,-42,15,15,15,-25,15,15,-26,36,36,15,-48,36,15,-56,-57,36,-11,-12,15,-14,15,-15,-37,-40,-27,-38,-39,36,-46,15,-34,36,-54,15,15,-16,-17,-43,-47,36,-33,15,-55,36,36,]),'MINUS':([9,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,44,46,48,49,50,52,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,71,72,73,74,75,76,77,78,79,80,81,82,83,85,86,],[17,37,17,-13,17,17,-18,-19,-20,-21,-22,-23,-24,17,-28,-29,-30,-31,-32,17,-57,-42,17,17,17,-25,17,17,-26,37,37,17,-48,37,17,-56,-57,37,-11,-12,17,-14,17,-15,-37,-40,-27,-38,-39,37,-46,17,-34,37,-54,17,17,-16,-17,-43,-47,37,-33,17,-55,37,37,]),'LPAREN':([9,15,17,18,26,32,34,35,36,37,39,40,46,50,58,60,63,66,69,74,75,82,],[26,26,26,26,26,26,50,26,26,26,26,26,26,26,26,26,50,50,26,26,26,26,]),'STRING':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,27,]),'BOOL':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,28,]),'NONE':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,29,]),'LARRAY':([9,15,17,18,26,30,31,32,34,35,36,37,39,40,46,50,58,60,62,63,65,66,69,71,74,75,78,81,82,],[32,32,32,32,32,46,-41,32,-42,32,32,32,32,32,32,32,32,32,-37,-40,-38,-39,32,-34,32,32,-43,-33,32,]),'ID':([9,15,17,18,26,32,35,36,37,39,40,43,45,46,50,58,60,69,74,75,82,],[34,34,34,34,34,34,34,34,34,34,34,63,66,34,34,34,34,34,34,34,34,]),'LDICT':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[35,35,35,35,35,35,35,35,35,35,35,35,35,35,35,35,35,35,35,]),'RPAREN':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,44,48,50,52,56,57,59,61,62,63,64,65,66,68,70,71,72,73,76,77,78,79,81,83,86,],[-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,64,-48,71,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,81,-34,-36,-54,-16,-17,-43,-47,-33,-55,-35,]),'RARRAY':([16,19,20,21,22,23,24,25,27,28,29,30,31,32,33,34,38,41,42,47,48,49,52,56,57,59,61,62,63,64,65,66,67,68,69,71,73,76,77,78,79,80,81,83,],[-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,48,-57,-42,-25,-26,-51,68,-48,-45,-56,-11,-12,-14,-15,-37,-40,-27,-38,-39,78,-46,79,-34,-54,-16,-17,-43,-47,-44,-33,-55,]),'COMMA':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,47,48,49,51,52,53,54,56,57,59,61,62,63,64,65,66,68,70,71,72,73,76,77,78,79,80,81,83,84,85,86,],[-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,69,-48,-45,74,-56,-50,-52,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,82,-34,-36,-54,-16,-17,-43,-47,-44,-33,-55,-49,-53,-35,]),'COLON':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,42,48,52,54,55,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,-26,-51,-48,-56,-57,75,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'RDICT':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,35,38,41,42,48,51,52,53,54,56,57,59,61,62,63,64,65,66,68,71,73,74,76,77,78,79,81,83,84,85,],[-13,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,52,-25,-26,-51,-48,73,-56,-50,-52,-11,-12,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,83,-16,-17,-43,-47,-33,-55,-49,-53,]),'TIMES':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,39,41,48,52,54,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[39,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,58,-26,-48,-56,-57,39,39,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'DIVIDE':([16,19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,40,41,48,52,54,56,57,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[40,-18,-19,-20,-21,-22,-23,-24,-28,-29,-30,-31,-32,-57,-42,-25,60,-26,-48,-56,-57,40,40,-14,-15,-37,-40,-27,-38,-39,-46,-34,-54,-16,-17,-43,-47,-33,-55,]),'DOT':([19,20,21,22,23,24,25,27,28,29,30,31,33,34,38,41,48,52,54,59,61,62,63,64,65,66,68,71,73,76,77,78,79,81,83,],[43,-19,-20,-21,-22,-23,-24,-28,-29,-30,45,-32,-57,-42,-25,-26,-48,-56,-57,43,43,-37,-40,-27,-38,-39,-46,-34,-54,43,43,-43,-47,-33,-55,]),}
+
+_lr_action = {}
+for _k, _v in _lr_action_items.items():
+   for _x,_y in zip(_v[0],_v[1]):
+      if not _x in _lr_action:  _lr_action[_x] = {}
+      _lr_action[_x][_k] = _y
+del _lr_action_items
+
+_lr_goto_items = {'master':([0,],[1,]),'block':([0,1,3,5,],[2,4,8,13,]),'blockcontent':([3,],[5,]),'attr':([3,5,],[7,12,]),'expr':([9,18,26,32,35,46,50,69,74,75,82,],[14,42,44,49,55,67,72,80,55,85,86,]),'term':([9,18,26,32,35,36,37,46,50,69,74,75,82,],[16,16,16,16,16,56,57,16,16,16,16,16,16,]),'factor':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[19,38,41,19,19,19,19,19,19,59,61,19,19,76,77,19,19,19,19,]),'identifier':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,30,]),'func':([9,15,17,18,26,32,35,36,37,39,40,43,45,46,50,58,60,69,74,75,82,],[31,31,31,31,31,31,31,31,31,31,31,62,65,31,31,31,31,31,31,31,31,]),'dict':([9,15,17,18,26,32,35,36,37,39,40,46,50,58,60,69,74,75,82,],[33,33,33,33,33,33,54,33,33,33,33,33,33,33,33,33,33,33,33,]),'arraydata':([32,],[47,]),'dictdata':([35,],[51,]),'dictcouple':([35,74,],[53,84,]),'funcargs':([50,],[70,]),}
+
+_lr_goto = {}
+for _k, _v in _lr_goto_items.items():
+   for _x, _y in zip(_v[0], _v[1]):
+       if not _x in _lr_goto: _lr_goto[_x] = {}
+       _lr_goto[_x][_k] = _y
+del _lr_goto_items
+_lr_productions = [
+  ("S' -> master","S'",1,None,None,None),
+  ('master -> master block','master',2,'p_master','parser.py',40),
+  ('master -> block','master',1,'p_master','parser.py',41),
+  ('block -> CLASS blockcontent END','block',3,'p_block','parser.py',52),
+  ('block -> CLASS END','block',2,'p_block','parser.py',53),
+  ('blockcontent -> blockcontent attr','blockcontent',2,'p_blockcontent','parser.py',70),
+  ('blockcontent -> blockcontent block','blockcontent',2,'p_blockcontent','parser.py',71),
+  ('blockcontent -> attr','blockcontent',1,'p_blockcontent','parser.py',72),
+  ('blockcontent -> block','blockcontent',1,'p_blockcontent','parser.py',73),
+  ('attr -> ATTR expr','attr',2,'p_attrset','parser.py',91),
+  ('attr -> BODY','attr',1,'p_attrset','parser.py',92),
+  ('expr -> expr PLUS term','expr',3,'p_binops','parser.py',102),
+  ('expr -> expr MINUS term','expr',3,'p_binops','parser.py',103),
+  ('expr -> term','expr',1,'p_binops','parser.py',104),
+  ('term -> term TIMES factor','term',3,'p_binops','parser.py',105),
+  ('term -> term DIVIDE factor','term',3,'p_binops','parser.py',106),
+  ('term -> term TIMES TIMES factor','term',4,'p_binops','parser.py',107),
+  ('term -> term DIVIDE DIVIDE factor','term',4,'p_binops','parser.py',108),
+  ('term -> factor','term',1,'p_binops','parser.py',109),
+  ('factor -> NUM_INT','factor',1,'p_factor_num','parser.py',124),
+  ('factor -> NUM_FLOAT','factor',1,'p_factor_num','parser.py',125),
+  ('factor -> NUM_HEX','factor',1,'p_factor_num','parser.py',126),
+  ('factor -> NUM_OCT','factor',1,'p_factor_num','parser.py',127),
+  ('factor -> NUM_IMAG','factor',1,'p_factor_num','parser.py',128),
+  ('factor -> NUM_BIN','factor',1,'p_factor_num','parser.py',129),
+  ('factor -> PLUS factor','factor',2,'p_factor_num','parser.py',130),
+  ('factor -> MINUS factor','factor',2,'p_factor_num','parser.py',131),
+  ('factor -> LPAREN expr RPAREN','factor',3,'p_factor_paren_expr','parser.py',140),
+  ('factor -> STRING','factor',1,'p_factor_str','parser.py',146),
+  ('factor -> BOOL','factor',1,'p_factor_bool','parser.py',152),
+  ('factor -> NONE','factor',1,'p_factor_none','parser.py',157),
+  ('factor -> identifier','factor',1,'p_factor_id','parser.py',163),
+  ('factor -> func','factor',1,'p_factor_id','parser.py',164),
+  ('func -> ID LPAREN funcargs RPAREN','func',4,'p_func','parser.py',169),
+  ('func -> ID LPAREN RPAREN','func',3,'p_func','parser.py',170),
+  ('funcargs -> funcargs COMMA expr','funcargs',3,'p_funcargs','parser.py',178),
+  ('funcargs -> expr','funcargs',1,'p_funcargs','parser.py',179),
+  ('identifier -> factor DOT func','identifier',3,'p_id_func','parser.py',188),
+  ('identifier -> identifier DOT func','identifier',3,'p_id_func','parser.py',189),
+  ('identifier -> identifier DOT ID','identifier',3,'p_id','parser.py',194),
+  ('identifier -> factor DOT ID','identifier',3,'p_id','parser.py',195),
+  ('identifier -> func','identifier',1,'p_id','parser.py',196),
+  ('identifier -> ID','identifier',1,'p_id','parser.py',197),
+  ('identifier -> identifier LARRAY expr RARRAY','identifier',4,'p_id_index','parser.py',209),
+  ('arraydata -> arraydata COMMA expr','arraydata',3,'p_arraydata','parser.py',216),
+  ('arraydata -> expr','arraydata',1,'p_arraydata','parser.py',217),
+  ('factor -> LARRAY arraydata RARRAY','factor',3,'p_factor_arr','parser.py',227),
+  ('factor -> LARRAY arraydata COMMA RARRAY','factor',4,'p_factor_arr','parser.py',228),
+  ('factor -> LARRAY RARRAY','factor',2,'p_factor_arr','parser.py',229),
+  ('dictdata -> dictdata COMMA dictcouple','dictdata',3,'p_dictdata','parser.py',238),
+  ('dictdata -> dictcouple','dictdata',1,'p_dictdata','parser.py',239),
+  ('expr -> NOT expr','expr',2,'p_not','parser.py',248),
+  ('dictdata -> dict','dictdata',1,'p_dict_dictdata','parser.py',253),
+  ('dictcouple -> expr COLON expr','dictcouple',3,'p_factor_dictcouple','parser.py',258),
+  ('dict -> LDICT dictdata RDICT','dict',3,'p_factor_dict','parser.py',263),
+  ('dict -> LDICT dictdata COMMA RDICT','dict',4,'p_factor_dict','parser.py',264),
+  ('dict -> LDICT RDICT','dict',2,'p_factor_dict','parser.py',265),
+  ('factor -> dict','factor',1,'p_dict','parser.py',270),
+]
```

### Comparing `e3lm-0.1.8/src/e3lm/tests/test_interpreters.py` & `e3lm-0.1.9/src/e3lm/tests/test_interpreters.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import pytest
-from e3lm.helpers import printers
-from e3lm.lang import ast
-from e3lm.demos import data
-from e3lm.lang.lexer import E3lmLexer
-from e3lm.lang.parser import E3lmParser
-from e3lm.utils.lang import interpret
-from e3lm.lang.interpreters import dot_get
-
-lexer = E3lmLexer()
-parser = E3lmParser()
-
-
-def test_basic_interpret():
-    for i, d in enumerate(data.examples):
-        if "interpret" not in d.keys():
-            continue
-        printers.cprint("test_interpreters: Code "+str(i))
-        lexer.build(debug=0)
-        parser.build(debug=0, lexer=lexer, tracking=True)
-        er = None
-        try:
-            program = interpret(d["text"], parser=parser)
-        except (IndentationError,
-                SyntaxError, AttributeError, ValueError,
-                NotImplementedError, IndexError, TypeError) as e:
-            er = e
-
-        if type(d["interpret"]) == dict:
-            _d = d["interpret"]
-            if "assert" in _d.keys():
-                for a in _d["assert"]:
-                    if a[0] == "error":
-                        if er != None:
-                            if "class" in a[1].keys():
-                                assert er.__class__.__name__ == a[1]["class"]
-                            if "lineno" in a[1].keys():
-                                assert er.lineno == a[1]["lineno"]
-                        else:
-                            raise AssertionError(
-                                "Code did not raise {} error."
-                                .format(a[1]["class"])
-                            )
-                    else:
-                        if er == None:
-                            dot = dot_get(program, a[0], eval=True)
-                            assert dot == a[1]
-                        else:
-                            raise AssertionError("No program.")
+import pytest
+from e3lm.helpers import printers
+from e3lm.lang import ast
+from e3lm.demos import data
+from e3lm.lang.lexer import E3lmLexer
+from e3lm.lang.parser import E3lmParser
+from e3lm.utils.lang import interpret
+from e3lm.lang.interpreters import dot_get
+
+lexer = E3lmLexer()
+parser = E3lmParser()
+
+
+def test_basic_interpret():
+    for i, d in enumerate(data.examples):
+        if "interpret" not in d.keys():
+            continue
+        printers.cprint("test_interpreters: Code "+str(i))
+        lexer.build(debug=0)
+        parser.build(debug=0, lexer=lexer, tracking=True)
+        er = None
+        try:
+            program = interpret(d["text"], parser=parser)
+        except (IndentationError,
+                SyntaxError, AttributeError, ValueError,
+                NotImplementedError, IndexError, TypeError) as e:
+            er = e
+
+        if type(d["interpret"]) == dict:
+            _d = d["interpret"]
+            if "assert" in _d.keys():
+                for a in _d["assert"]:
+                    if a[0] == "error":
+                        if er != None:
+                            if "class" in a[1].keys():
+                                assert er.__class__.__name__ == a[1]["class"]
+                            if "lineno" in a[1].keys():
+                                assert er.lineno == a[1]["lineno"]
+                        else:
+                            raise AssertionError(
+                                "Code did not raise {} error."
+                                .format(a[1]["class"])
+                            )
+                    else:
+                        if er == None:
+                            dot = dot_get(program, a[0], eval=True)
+                            assert dot == a[1]
+                        else:
+                            raise AssertionError("No program.")
```

### Comparing `e3lm-0.1.8/src/e3lm/tests/test_lexer.py` & `e3lm-0.1.9/src/e3lm/tests/test_lexer.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import pytest
-from e3lm.helpers import printers
-from e3lm.demos import data
-from e3lm.lang.lexer import E3lmLexer
-from e3lm.utils.lang import lex
-
-lexer = E3lmLexer()
-
-
-def test_lexer():
-    for i, d in enumerate(data.examples):
-        if "lex" not in d.keys():
-            continue
-
-        with_stmt = False
-        print(d["raises"], i, d["ind"])
-        if "raises" in d.keys():
-            with_stmt = "lex" in d["raises"]
-            print(with_stmt)
-
-        lexer.build(debug=0)
-        er = None
-        if with_stmt:
-            with pytest.raises((IndentationError, SyntaxError,)) as e:
-                lexed = lex(d["text"], lexer=lexer,
-                            source=str(i)+":"+str(d["ind"]))
-                toks = [t.type for t in lexed]
-            er = e.value
-        else:
-            lexed = lex(d["text"], lexer=lexer,
-                        source=str(i)+":"+str(d["ind"]))
-            toks = [t.type for t in lexed]
-
-        if type(d["lex"]) == dict:
-            _d = d["lex"]
-            if "assert" in _d.keys():
-                for a in _d["assert"]:
-                    if a[0] == "tokens":
-                        assert toks == a[1]
-                    elif a[0] == "error":
-                        if er != None:
-                            if "class" in a[1].keys():
-                                assert er.__class__.__name__ == a[1]["class"]
-                            if "lineno" in a[1].keys():
-                                assert er.lineno == a[1]["lineno"]
-                        else:
-                            raise AssertionError(
-                                "Code {} did not raise {} error."
-                                .format(str(i), a[1]["class"])
-                            )
+import pytest
+from e3lm.helpers import printers
+from e3lm.demos import data
+from e3lm.lang.lexer import E3lmLexer
+from e3lm.utils.lang import lex
+
+lexer = E3lmLexer()
+
+
+def test_lexer():
+    for i, d in enumerate(data.examples):
+        if "lex" not in d.keys():
+            continue
+
+        with_stmt = False
+        print(d["raises"], i, d["ind"])
+        if "raises" in d.keys():
+            with_stmt = "lex" in d["raises"]
+            print(with_stmt)
+
+        lexer.build(debug=0)
+        er = None
+        if with_stmt:
+            with pytest.raises((IndentationError, SyntaxError,)) as e:
+                lexed = lex(d["text"], lexer=lexer,
+                            source=str(i)+":"+str(d["ind"]))
+                toks = [t.type for t in lexed]
+            er = e.value
+        else:
+            lexed = lex(d["text"], lexer=lexer,
+                        source=str(i)+":"+str(d["ind"]))
+            toks = [t.type for t in lexed]
+
+        if type(d["lex"]) == dict:
+            _d = d["lex"]
+            if "assert" in _d.keys():
+                for a in _d["assert"]:
+                    if a[0] == "tokens":
+                        assert toks == a[1]
+                    elif a[0] == "error":
+                        if er != None:
+                            if "class" in a[1].keys():
+                                assert er.__class__.__name__ == a[1]["class"]
+                            if "lineno" in a[1].keys():
+                                assert er.lineno == a[1]["lineno"]
+                        else:
+                            raise AssertionError(
+                                "Code {} did not raise {} error."
+                                .format(str(i), a[1]["class"])
+                            )
```

### Comparing `e3lm-0.1.8/src/e3lm/tests/test_parser.py` & `e3lm-0.1.9/src/e3lm/tests/test_parser.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import pytest
-from e3lm.helpers import printers
-from e3lm.demos import data
-from e3lm.lang.parser import E3lmParser
-from e3lm.utils.lang import parse
-
-parser = E3lmParser()
-
-
-def test_parser_errors():
-    for i, d in enumerate(data.examples):
-        if "parse" not in d.keys():
-            continue
-        printers.cprint("test_parser: Code "+str(i))
-        parser.build(debug=1)
-        er = None
-        try:
-            parsed = parse(d["text"], parser=parser, debug=0, tracking=True)
-        except (IndentationError, SyntaxError) as e:
-            er = e
-
-        if type(d["parse"]) == dict:
-            _d = d["parse"]
-            if "assert" in _d.keys():
-                passerts = 0
-                passerts_count = len([pe for pe in _d['assert']
-                                      if pe[0] == "p_error"])
-                for a in _d["assert"]:
-                    if a[0] == "error":
-                        if er != None:
-                            if "class" in a[1].keys():
-                                assert er.__class__.__name__ == a[1]["class"]
-                            if "lineno" in a[1].keys():
-                                assert er.lineno == a[1]["lineno"]
-                        else:
-                            raise AssertionError(
-                                "Code {} did not raise {} error."
-                                .format(str(i), a[1]["class"])
-                            )
-                    elif a[0] == "p_error":
-                        for i, er in enumerate(parser.errors):
-                            asserted = False
-                            if "class" in a[1].keys():
-                                if er[0][0].__name__ == a[1]["class"]:
-                                    if "lineno" in a[1].keys():
-                                        if er[0][2] == a[1]["lineno"]:
-                                            asserted = True
-
-                            if asserted:
-                                passerts += 1
-                            # else:
-                            #     print(er[0][0].__name__, er[0][2])
-
-                assert passerts == passerts_count
+import pytest
+from e3lm.helpers import printers
+from e3lm.demos import data
+from e3lm.lang.parser import E3lmParser
+from e3lm.utils.lang import parse
+
+parser = E3lmParser()
+
+
+def test_parser_errors():
+    for i, d in enumerate(data.examples):
+        if "parse" not in d.keys():
+            continue
+        printers.cprint("test_parser: Code "+str(i))
+        parser.build(debug=1)
+        er = None
+        try:
+            parsed = parse(d["text"], parser=parser, debug=0, tracking=True)
+        except (IndentationError, SyntaxError) as e:
+            er = e
+
+        if type(d["parse"]) == dict:
+            _d = d["parse"]
+            if "assert" in _d.keys():
+                passerts = 0
+                passerts_count = len([pe for pe in _d['assert']
+                                      if pe[0] == "p_error"])
+                for a in _d["assert"]:
+                    if a[0] == "error":
+                        if er != None:
+                            if "class" in a[1].keys():
+                                assert er.__class__.__name__ == a[1]["class"]
+                            if "lineno" in a[1].keys():
+                                assert er.lineno == a[1]["lineno"]
+                        else:
+                            raise AssertionError(
+                                "Code {} did not raise {} error."
+                                .format(str(i), a[1]["class"])
+                            )
+                    elif a[0] == "p_error":
+                        for i, er in enumerate(parser.errors):
+                            asserted = False
+                            if "class" in a[1].keys():
+                                if er[0][0].__name__ == a[1]["class"]:
+                                    if "lineno" in a[1].keys():
+                                        if er[0][2] == a[1]["lineno"]:
+                                            asserted = True
+
+                            if asserted:
+                                passerts += 1
+                            # else:
+                            #     print(er[0][0].__name__, er[0][2])
+
+                assert passerts == passerts_count
```

### Comparing `e3lm-0.1.8/src/e3lm/tests/test_utils.py` & `e3lm-0.1.9/src/e3lm/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from e3lm.lang.interpreters import (
-    E3lmInterpreter,
-    get_attr, dot_get,
-)
-from e3lm.lang import ast
-from e3lm.utils.lang import interpret
-from e3lm.lang.lexer import E3lmLexer
-from e3lm.lang.parser import E3lmParser
-from e3lm.demos import data
-
-
-def test_backflow():
-    block1 = ast.Block("Dummy", attrs={
-        "attr1": ast.Attr("attr1", 0)
-    }, name="block1")
-
-    block2 = ast.Block("Dummy")
-    block3 = ast.Block("Dummy")
-
-    blocks = [
-        block1,
-        block2,
-        block3,
-    ]
-
-    program = ast.Program(blocks=blocks)
-    program.build_flat()
-    assert block1 == get_attr(program, "block1")
-
-
-def test_dotget():
-    program = interpret(data.code4)
-    assert "hello" == dot_get(program, "my1.attr2.0.1.2.hi")
+from e3lm.lang.interpreters import (
+    E3lmInterpreter,
+    get_attr, dot_get,
+)
+from e3lm.lang import ast
+from e3lm.utils.lang import interpret
+from e3lm.lang.lexer import E3lmLexer
+from e3lm.lang.parser import E3lmParser
+from e3lm.demos import data
+
+
+def test_backflow():
+    block1 = ast.Block("Dummy", attrs={
+        "attr1": ast.Attr("attr1", 0)
+    }, name="block1")
+
+    block2 = ast.Block("Dummy")
+    block3 = ast.Block("Dummy")
+
+    blocks = [
+        block1,
+        block2,
+        block3,
+    ]
+
+    program = ast.Program(blocks=blocks)
+    program.build_flat()
+    assert block1 == get_attr(program, "block1")
+
+
+def test_dotget():
+    program = interpret(data.code4)
+    assert "hello" == dot_get(program, "my1.attr2.0.1.2.hi")
```

### Comparing `e3lm-0.1.8/src/e3lm/utils/lang.py` & `e3lm-0.1.9/src/e3lm/utils/lang.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-"""
-Author: Kenan Masri
-
-"""
-
-import json
-import types
-import inspect as _inspect
-from e3lm.helpers.printers import cprint
-from e3lm.lang.parser import E3lmParser
-from e3lm.lang.lexer import E3lmLexer
-from e3lm.lang.interpreters import E3lmInterpreter
-
-_lexer = E3lmLexer()
-_parser = E3lmParser()
-
-
-def lex(text, source=None, lexer=None, token_map=True, **kwargs):
-    """Lex text.
-
-    `lexer`, `source` and the rest are used for building the lexer
-    """
-    srs = source or "<string>"
-
-    if not lexer:
-        l = _lexer
-    else:
-        l = lexer
-        if _inspect.isclass(l):
-            l = l()
-
-    l.build(**kwargs)
-    l.input(text, srs)
-    if token_map:
-        tokens = l.get_tokens()
-        tokmap = []
-        for tok in tokens:
-            tokmap.append(tok)
-        return tokmap
-    else:
-        return l.token
-
-
-def parse(text, source=None,
-          lexer=None, lexer_kwargs={},
-          parser=None, parser_kwargs={},
-          **kwargs
-          ):  # pragma: no cover
-
-    lexer = lexer \
-        or (1 if "lexer" in parser_kwargs.keys() else None)\
-        or _lexer
-    if lexer == 1:
-        lexer = parser_kwargs.pop("lexer")
-
-    parser = parser or _parser
-    lexer_kwargs = lexer_kwargs \
-        or (parser_kwargs["lexer_kwargs"]
-            if "lexer_kwargs" in parser_kwargs.keys() else {})
-
-    parse_kwargs = kwargs \
-        or (parser_kwargs["parse_kwargs"]
-            if "parse_kwargs" in parser_kwargs.keys() else {})
-
-    lexer.build(**lexer_kwargs)
-    parser.build(lexer=lexer, **parser_kwargs)
-
-    return parser.parse(text, source, **kwargs)
-
-
-def interpret(text, source=None,
-              interpreter_cls=E3lmInterpreter,
-              parser=None, parser_kwargs={},
-              plugins=[],
-              **kwargs
-              ):  # pragma: no cover
-
-    p = parser or _parser
-    if _inspect.isclass(p):
-        p = p()
-    p.build(**parser_kwargs)
-
-    pre_interpreter = interpreter_cls(parser=p)
-
-    # PRE E3lm
-    result = pre_interpreter.interpret(text, source)
-    pipe = [pre_interpreter.__class__.__name__]
-
-    if result == None:
-        return None
-
-    worked = []
-    for plugin in plugins:
-        if _inspect.isclass(plugin):
-            plugin = plugin()
-            plugin.is_plugin = True
-            plugin.is_pre = True
-            plugin.is_post = False
-        _result = plugin.interpret(result, source)
-        if _result:
-            result = _result
-            worked.append(plugin)
-            pipe.append(plugin.__class__.__name__)
-        elif _result == None:
-            raise BrokenPipeError(1, pipe, "Could not continue pipe.")
-
-    for plugin in worked:
-        if hasattr(plugin, "post_process"):
-            result = plugin.post_process(result)
-            if result == None:
-                raise ValueError("'{}' post_process did not return Program."
-                                 .format(plugin.__class__.__name__))
-
-    return result
-
-
-def get_plugin(string):
-    """Gets an E3lm plugin from the plugins contrib folder or a directory
-    specified by the env variable `E3LM_PYTHON_PLUGINS_DIR`.
-
-    Plugins are classes that extend E3lmPlugin and the file name is the
-    plugin name. For example "json" plugin is from the file "json.py"
-    and the class name is JsonPlugin. The class name is the plugin name
-    but the first letter is uppercased plus "Plugin".
-
-    If the custom plugin folder does not have __init__.py, it is ignored and
-    fallbacks to E3lmPlugin default directory.
-    """
-    import os
-    res = {}
-    dirs = []
-    os.environ.setdefault(
-        "E3LM_PYTHON_PLUGINS_DIR", "e3lm_plugins")
-    pluginsdir = os.environ.get("E3LM_PYTHON_PLUGINS_DIR")
-    if not os.path.exists(pluginsdir) or not os.path.isdir(pluginsdir):
-        pluginsdir = os.path.abspath(os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), '..' + os.sep, 'contrib'))
-
-    if not os.path.isdir(pluginsdir) or not os.path.exists(pluginsdir + os.sep + "__init__.py"):
-        pluginsdir = os.path.abspath(os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), '..' + os.sep, 'contrib'))
-
-    if not os.path.isdir(pluginsdir) or not os.path.exists(pluginsdir + os.sep + "__init__.py"):
-        raise ImportError("E3lm cannot find plugin \"" + str(string) +
-                          "\" in the plugins dir \"" + pluginsdir + "\".")
-
-    if not string.endswith(".py"):
-        string = string + ".py"
-    if os.path.exists(pluginsdir + os.sep + string):
-        if not os.path.isfile(pluginsdir + os.sep + string):
-            raise ImportError("E3lm cannot import directory as plugin \"" +
-                              str(string) + "\" in the plugins dir \"" + pluginsdir + "\".")
-        try:
-            module = __import__("e3lm.contrib." + string[:-3], fromlist=["*"])
-            x = getattr(module, string[0].upper() + string[1:-3] + "Plugin")
-            return x
-        except ImportError as e:
-            raise e
-        except AttributeError as e:
-            raise e
+"""
+Author: Kenan Masri
+
+"""
+
+import json
+import types
+import inspect as _inspect
+from e3lm.helpers.printers import cprint
+from e3lm.lang.parser import E3lmParser
+from e3lm.lang.lexer import E3lmLexer
+from e3lm.lang.interpreters import E3lmInterpreter
+
+_lexer = E3lmLexer()
+_parser = E3lmParser()
+
+
+def lex(text, source=None, lexer=None, token_map=True, **kwargs):
+    """Lex text.
+
+    `lexer`, `source` and the rest are used for building the lexer
+    """
+    srs = source or "<string>"
+
+    if not lexer:
+        l = _lexer
+    else:
+        l = lexer
+        if _inspect.isclass(l):
+            l = l()
+
+    l.build(**kwargs)
+    l.input(text, srs)
+    if token_map:
+        tokens = l.get_tokens()
+        tokmap = []
+        for tok in tokens:
+            tokmap.append(tok)
+        return tokmap
+    else:
+        return l.token
+
+
+def parse(text, source=None,
+          lexer=None, lexer_kwargs={},
+          parser=None, parser_kwargs={},
+          **kwargs
+          ):  # pragma: no cover
+
+    lexer = lexer \
+        or (1 if "lexer" in parser_kwargs.keys() else None)\
+        or _lexer
+    if lexer == 1:
+        lexer = parser_kwargs.pop("lexer")
+
+    parser = parser or _parser
+    lexer_kwargs = lexer_kwargs \
+        or (parser_kwargs["lexer_kwargs"]
+            if "lexer_kwargs" in parser_kwargs.keys() else {})
+
+    parse_kwargs = kwargs \
+        or (parser_kwargs["parse_kwargs"]
+            if "parse_kwargs" in parser_kwargs.keys() else {})
+
+    lexer.build(**lexer_kwargs)
+    parser.build(lexer=lexer, **parse_kwargs)
+
+    return parser.parse(text, source, **kwargs)
+
+
+def interpret(text, source=None,
+              interpreter_cls=E3lmInterpreter,
+              parser=None, parser_kwargs={},
+              plugins=[],
+              **kwargs
+              ):  # pragma: no cover
+
+    p = parser or _parser
+    if _inspect.isclass(p):
+        p = p()
+    p.build(**parser_kwargs)
+
+    pre_interpreter = interpreter_cls(parser=p)
+
+    # PRE E3lm
+    result = pre_interpreter.interpret(text, source)
+    pipe = [pre_interpreter.__class__.__name__]
+
+    if result == None:
+        return None
+
+    worked = []
+    for plugin in plugins:
+        if _inspect.isclass(plugin):
+            plugin = plugin()
+            plugin.is_plugin = True
+            plugin.is_pre = True
+            plugin.is_post = False
+        _result = plugin.interpret(result, source)
+        if _result:
+            result = _result
+            worked.append(plugin)
+            pipe.append(plugin.__class__.__name__)
+        elif _result == None:
+            raise BrokenPipeError(1, pipe, "Could not continue pipe.")
+
+    for plugin in worked:
+        if hasattr(plugin, "post_process"):
+            result = plugin.post_process(result)
+            if result == None:
+                raise ValueError("'{}' post_process did not return Program."
+                                 .format(plugin.__class__.__name__))
+
+    return result
+
+
+def get_plugin(string):
+    """Gets an E3lm plugin from the plugins contrib folder or a directory
+    specified by the env variable `E3LM_PYTHON_PLUGINS_DIR`.
+
+    Plugins are classes that extend E3lmPlugin and the file name is the
+    plugin name. For example "json" plugin is from the file "json.py"
+    and the class name is JsonPlugin. The class name is the plugin name
+    but the first letter is uppercased plus "Plugin".
+
+    If the custom plugin folder does not have __init__.py, it is ignored and
+    fallbacks to E3lmPlugin default directory.
+    """
+    import os
+    res = {}
+    dirs = []
+    os.environ.setdefault(
+        "E3LM_PYTHON_PLUGINS_DIR", "e3lm_plugins")
+    pluginsdir = os.environ.get("E3LM_PYTHON_PLUGINS_DIR")
+    if not os.path.exists(pluginsdir) or not os.path.isdir(pluginsdir):
+        pluginsdir = os.path.abspath(os.path.join(os.path.dirname(
+            os.path.realpath(__file__)), '..' + os.sep, 'contrib'))
+
+    if not os.path.isdir(pluginsdir) or not os.path.exists(pluginsdir + os.sep + "__init__.py"):
+        pluginsdir = os.path.abspath(os.path.join(os.path.dirname(
+            os.path.realpath(__file__)), '..' + os.sep, 'contrib'))
+
+    if not os.path.isdir(pluginsdir) or not os.path.exists(pluginsdir + os.sep + "__init__.py"):
+        raise ImportError("E3lm cannot find plugin \"" + str(string) +
+                          "\" in the plugins dir \"" + pluginsdir + "\".")
+
+    if not string.endswith(".py"):
+        string = string + ".py"
+    if os.path.exists(pluginsdir + os.sep + string):
+        if not os.path.isfile(pluginsdir + os.sep + string):
+            raise ImportError("E3lm cannot import directory as plugin \"" +
+                              str(string) + "\" in the plugins dir \"" + pluginsdir + "\".")
+        try:
+            module = __import__("e3lm.contrib." + string[:-3], fromlist=["*"])
+            x = getattr(module, string[0].upper() + string[1:-3] + "Plugin")
+            return x
+        except ImportError as e:
+            raise e
+        except AttributeError as e:
+            raise e
     raise ModuleNotFoundError("Could not find e3lm plugin \"" + str(string[:-3]) + "\".")
```

### Comparing `e3lm-0.1.8/src/e3lm/utils/spin.py` & `e3lm-0.1.9/src/e3lm/utils/spin.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""
-A module for showing Luxembourgish braille dots
-as a progress bar or spinner.
-"""
-
-__author__ = "Kenan Masri"
-__version__ = "0.1.0"
-__license__ = "MIT"
-
-import itertools
-import argparse
-import time
-import sys
-
-def animate(message, speed=0.033):
-    for c in itertools.cycle([ 
-        '⡀','⠄','⠂','⠁','⠈','⠐','⠠','⢀', # Luxembourgish braille dots :D
-    ]):
-        sys.stdout.write('\r' + c + ' ' + message)
-        sys.stdout.flush()
-        time.sleep(0.033)
-
-if __name__ == "__main__":
-    args = sys.argv
-    message = ""
-    speed = args[2] if len(args) >= 3 else 0.033
-
-    sys.stdout.flush()
-    while True:
-        animate(message, speed=speed)
-        time.sleep(0.001)
+"""
+A module for showing Luxembourgish braille dots
+as a progress bar or spinner.
+"""
+
+__author__ = "Kenan Masri"
+__version__ = "0.1.0"
+__license__ = "MIT"
+
+import itertools
+import argparse
+import time
+import sys
+
+def animate(message, speed=0.033):
+    for c in itertools.cycle([ 
+        '⡀','⠄','⠂','⠁','⠈','⠐','⠠','⢀', # Luxembourgish braille dots :D
+    ]):
+        sys.stdout.write('\r' + c + ' ' + message)
+        sys.stdout.flush()
+        time.sleep(0.033)
+
+if __name__ == "__main__":
+    args = sys.argv
+    message = ""
+    speed = args[2] if len(args) >= 3 else 0.033
+
+    sys.stdout.flush()
+    while True:
+        animate(message, speed=speed)
+        time.sleep(0.001)
```

### Comparing `e3lm-0.1.8/src/e3lm.egg-info/SOURCES.txt` & `e3lm-0.1.9/src/e3lm.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 src/e3lm.egg-info/dependency_links.txt
 src/e3lm.egg-info/entry_points.txt
 src/e3lm.egg-info/requires.txt
 src/e3lm.egg-info/top_level.txt
 src/e3lm/contrib/__init__.py
 src/e3lm/contrib/dot.py
 src/e3lm/contrib/json.py
-src/e3lm/contrib/ppt.py
 src/e3lm/contrib/units.py
 src/e3lm/demos/__init__.py
 src/e3lm/demos/data.py
 src/e3lm/helpers/__init__.py
 src/e3lm/helpers/printers.py
 src/e3lm/lang/__init__.py
 src/e3lm/lang/ast.py
```

