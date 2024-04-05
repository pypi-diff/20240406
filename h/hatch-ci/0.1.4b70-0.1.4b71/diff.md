# Comparing `tmp/hatch-ci-0.1.4b70.tar.gz` & `tmp/hatch-ci-0.1.4b71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatch-ci-0.1.4b70.tar", last modified: Fri Apr  5 19:39:46 2024, max compression
+gzip compressed data, was "hatch-ci-0.1.4b71.tar", last modified: Fri Apr  5 20:00:58 2024, max compression
```

## Comparing `hatch-ci-0.1.4b70.tar` & `hatch-ci-0.1.4b71.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:39:46.911744 hatch-ci-0.1.4b70/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-05 19:39:46.911744 hatch-ci-0.1.4b70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-05 19:39:44.000000 hatch-ci-0.1.4b70/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-05 19:39:44.000000 hatch-ci-0.1.4b70/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:39:46.911744 hatch-ci-0.1.4b70/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:39:46.903744 hatch-ci-0.1.4b70/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:39:46.907744 hatch-ci-0.1.4b70/src/hatch_ci/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/code.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/fileos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/hook_build.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/hook_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/hook_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/scm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/script.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/src/hatch_ci/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:39:46.911744 hatch-ci-0.1.4b70/src/hatch_ci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-05 19:39:46.000000 hatch-ci-0.1.4b70/src/hatch_ci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-05 19:39:46.000000 hatch-ci-0.1.4b70/src/hatch_ci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:39:46.000000 hatch-ci-0.1.4b70/src/hatch_ci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 19:39:46.000000 hatch-ci-0.1.4b70/src/hatch_ci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 19:39:46.000000 hatch-ci-0.1.4b70/src/hatch_ci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 19:39:46.000000 hatch-ci-0.1.4b70/src/hatch_ci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:39:46.911744 hatch-ci-0.1.4b70/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/tests/test_fileos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-04-05 19:39:06.000000 hatch-ci-0.1.4b70/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:00:58.377300 hatch-ci-0.1.4b71/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-05 20:00:58.377300 hatch-ci-0.1.4b71/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-05 20:00:55.000000 hatch-ci-0.1.4b71/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-05 20:00:55.000000 hatch-ci-0.1.4b71/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:00:58.377300 hatch-ci-0.1.4b71/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:00:58.365300 hatch-ci-0.1.4b71/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:00:58.369300 hatch-ci-0.1.4b71/src/hatch_ci/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/fileos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/hook_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/hook_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/hook_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/src/hatch_ci/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:00:58.377300 hatch-ci-0.1.4b71/src/hatch_ci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-05 20:00:58.000000 hatch-ci-0.1.4b71/src/hatch_ci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-05 20:00:58.000000 hatch-ci-0.1.4b71/src/hatch_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:00:58.000000 hatch-ci-0.1.4b71/src/hatch_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 20:00:58.000000 hatch-ci-0.1.4b71/src/hatch_ci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 20:00:58.000000 hatch-ci-0.1.4b71/src/hatch_ci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 20:00:58.000000 hatch-ci-0.1.4b71/src/hatch_ci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:00:58.373300 hatch-ci-0.1.4b71/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/tests/test_fileos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-04-05 20:00:09.000000 hatch-ci-0.1.4b71/tests/test_tools.py
```

### Comparing `hatch-ci-0.1.4b70/LICENSE.txt` & `hatch-ci-0.1.4b71/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/PKG-INFO` & `hatch-ci-0.1.4b71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.1.4b70
+Version: 0.1.4b71
 Summary: Hatch plugin for ci system versioning
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Keywords: git,hatch,plugin,scm,version
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,15 @@
 
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta/0.1.4.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
 [![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 > **NOTE** This is a beta branch!
```

### Comparing `hatch-ci-0.1.4b70/README.md` & `hatch-ci-0.1.4b71/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta/0.1.4.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
 [![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 > **NOTE** This is a beta branch!
```

### Comparing `hatch-ci-0.1.4b70/pyproject.toml` & `hatch-ci-0.1.4b71/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-__version__ = "0.1.4b70"
-__hash__ = "dad578e7fac5ef60a0c03986588fb2665e556272"
+__version__ = "0.1.4b71"
+__hash__ = "a579cbb4a161635b6011c244fa483b7d34b284f2"
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-ci"
-version = "0.1.4b70"
+version = "0.1.4b71"
 description = "Hatch plugin for ci system versioning"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">= 3.8"
 keywords = [
   "git",
   "hatch",
```

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/_support.py` & `hatch-ci-0.1.4b71/src/hatch_ci/_support.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/cli.py` & `hatch-ci-0.1.4b71/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/code.py` & `hatch-ci-0.1.4b71/src/hatch_ci/code.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/exceptions.py` & `hatch-ci-0.1.4b71/src/hatch_ci/exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/fileos.py` & `hatch-ci-0.1.4b71/src/hatch_ci/fileos.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/hook_build.py` & `hatch-ci-0.1.4b71/src/hatch_ci/hook_build.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/hook_version.py` & `hatch-ci-0.1.4b71/src/hatch_ci/hook_version.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/scm.py` & `hatch-ci-0.1.4b71/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/script.py` & `hatch-ci-0.1.4b71/src/hatch_ci/script.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/text.py` & `hatch-ci-0.1.4b71/src/hatch_ci/text.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci/tools.py` & `hatch-ci-0.1.4b71/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci.egg-info/PKG-INFO` & `hatch-ci-0.1.4b71/src/hatch_ci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.1.4b70
+Version: 0.1.4b71
 Summary: Hatch plugin for ci system versioning
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Keywords: git,hatch,plugin,scm,version
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,15 @@
 
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta/0.1.4.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
 [![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 > **NOTE** This is a beta branch!
```

### Comparing `hatch-ci-0.1.4b70/src/hatch_ci.egg-info/SOURCES.txt` & `hatch-ci-0.1.4b71/src/hatch_ci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/tests/test_cli.py` & `hatch-ci-0.1.4b71/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/tests/test_code.py` & `hatch-ci-0.1.4b71/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/tests/test_conftest.py` & `hatch-ci-0.1.4b71/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/tests/test_e2e.py` & `hatch-ci-0.1.4b71/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/tests/test_exceptions.py` & `hatch-ci-0.1.4b71/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/tests/test_fileos.py` & `hatch-ci-0.1.4b71/tests/test_fileos.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/tests/test_scm.py` & `hatch-ci-0.1.4b71/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/tests/test_script.py` & `hatch-ci-0.1.4b71/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/tests/test_text.py` & `hatch-ci-0.1.4b71/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b70/tests/test_tools.py` & `hatch-ci-0.1.4b71/tests/test_tools.py`

 * *Files identical despite different names*

