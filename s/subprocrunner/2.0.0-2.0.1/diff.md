# Comparing `tmp/subprocrunner-2.0.0.tar.gz` & `tmp/subprocrunner-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subprocrunner-2.0.0.tar", last modified: Sat Jan 15 12:56:57 2022, max compression
+gzip compressed data, was "subprocrunner-2.0.1.tar", last modified: Sat Apr  6 16:02:25 2024, max compression
```

## Comparing `subprocrunner-2.0.0.tar` & `subprocrunner-2.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-01-15 12:56:57.050000 subprocrunner-2.0.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      198 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     6800 2022-01-15 12:56:57.050000 subprocrunner-2.0.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     5223 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)      834 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-01-15 12:56:57.050000 subprocrunner-2.0.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       23 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       26 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2022-01-15 12:56:57.050000 subprocrunner-2.0.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2878 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-01-15 12:56:57.050000 subprocrunner-2.0.0/subprocrunner/
--rw-r--r--   0 toor      (1000) toor      (1000)      361 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/__version__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-01-15 12:56:57.050000 subprocrunner-2.0.0/subprocrunner/_logger/
--rw-r--r--   0 toor      (1000) toor      (1000)       92 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/_logger/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1297 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/_logger/_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1071 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/_logger/_null_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9976 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/_subprocess_runner.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1693 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/_which.py
--rw-r--r--   0 toor      (1000) toor      (1000)      605 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/error.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/py.typed
--rw-r--r--   0 toor      (1000) toor      (1000)     2117 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/retry.py
--rw-r--r--   0 toor      (1000) toor      (1000)       73 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/subprocrunner/typing.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-01-15 12:56:57.050000 subprocrunner-2.0.0/subprocrunner.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     6800 2022-01-15 12:56:56.000000 subprocrunner-2.0.0/subprocrunner.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      710 2022-01-15 12:56:56.000000 subprocrunner-2.0.0/subprocrunner.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-01-15 12:56:56.000000 subprocrunner-2.0.0/subprocrunner.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      102 2022-01-15 12:56:56.000000 subprocrunner-2.0.0/subprocrunner.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       14 2022-01-15 12:56:56.000000 subprocrunner-2.0.0/subprocrunner.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-01-15 12:56:57.050000 subprocrunner-2.0.0/test/
--rw-r--r--   0 toor      (1000) toor      (1000)      565 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/test/test_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1373 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/test/test_retry.py
--rw-r--r--   0 toor      (1000) toor      (1000)    10898 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/test/test_subproc_runner.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3346 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/test/test_which.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1121 2022-01-15 12:56:25.000000 subprocrunner-2.0.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-06 16:02:25.845052 subprocrunner-2.0.1/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      180 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     7637 2024-04-06 16:02:25.845052 subprocrunner-2.0.1/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     5664 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)     1473 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-06 16:02:25.835052 subprocrunner-2.0.1/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       23 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       26 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-04-06 16:02:25.845052 subprocrunner-2.0.1/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     3043 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-06 16:02:25.835052 subprocrunner-2.0.1/subprocrunner/
+-rw-r--r--   0 toor      (1000) toor      (1000)      605 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/__version__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-06 16:02:25.845052 subprocrunner-2.0.1/subprocrunner/_logger/
+-rw-r--r--   0 toor      (1000) toor      (1000)      204 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/_logger/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1296 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/_logger/_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1088 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/_logger/_null_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10427 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/_subprocess_runner.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1726 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/_which.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      619 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/py.typed
+-rw-r--r--   0 toor      (1000) toor      (1000)     2117 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/retry.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       73 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/subprocrunner/typing.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-06 16:02:25.845052 subprocrunner-2.0.1/subprocrunner.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     7637 2024-04-06 16:02:25.000000 subprocrunner-2.0.1/subprocrunner.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      710 2024-04-06 16:02:25.000000 subprocrunner-2.0.1/subprocrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-06 16:02:25.000000 subprocrunner-2.0.1/subprocrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      102 2024-04-06 16:02:25.000000 subprocrunner-2.0.1/subprocrunner.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       14 2024-04-06 16:02:25.000000 subprocrunner-2.0.1/subprocrunner.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-06 16:02:25.845052 subprocrunner-2.0.1/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)      564 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/test/test_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1373 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/test/test_retry.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11247 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/test/test_subproc_runner.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3401 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/test/test_which.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1364 2024-04-06 16:02:01.000000 subprocrunner-2.0.1/tox.ini
```

### Comparing `subprocrunner-2.0.0/LICENSE` & `subprocrunner-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `subprocrunner-2.0.0/PKG-INFO` & `subprocrunner-2.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,87 @@
 Metadata-Version: 2.1
 Name: subprocrunner
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python wrapper library for subprocess module.
 Home-page: https://github.com/thombashi/subprocrunner
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changlog, https://github.com/thombashi/subprocrunner/releases
 Project-URL: Source, https://github.com/thombashi/subprocrunner
 Project-URL: Tracker, https://github.com/thombashi/subprocrunner/issues
 Keywords: library,subprocess
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: mbstrdecoder<2,>=1.0.0
 Provides-Extra: logging
+Requires-Dist: loguru<1,>=0.4.1; extra == "logging"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+Requires-Dist: typepy; extra == "test"
+Requires-Dist: loguru<1,>=0.4.1; extra == "test"
 
 .. contents:: **subprocrunner**
    :backlinks: top
    :depth: 2
 
 
 Summary
 =============
 A Python wrapper library for ``subprocess`` module.
 
-.. image:: https://badge.fury.io/py/subprocrunner.svg
+|PyPI pkg ver| |Supported Python versions| |Supported Python implementations| |CI status| |Test coverage| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/subprocrunner.svg
     :target: https://badge.fury.io/py/subprocrunner
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/subprocrunner.svg
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/subprocrunner.svg
     :target: https://pypi.org/project/subprocrunner
     :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/implementation/subprocrunner.svg
+.. |Supported Python implementations| image:: https://img.shields.io/pypi/implementation/subprocrunner.svg
     :target: https://pypi.org/project/subprocrunner
     :alt: Supported Python implementations
 
-.. image:: https://github.com/thombashi/subprocrunner/actions/workflows/lint_and_test.yml/badge.svg
-    :target: https://github.com/thombashi/subprocrunner/actions/workflows/lint_and_test.yml
+.. |CI status| image:: https://github.com/thombashi/subprocrunner/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/subprocrunner/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://coveralls.io/repos/github/thombashi/subprocrunner/badge.svg?branch=master
+.. |Test coverage| image:: https://coveralls.io/repos/github/thombashi/subprocrunner/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/subprocrunner?branch=master
     :alt: Test coverage
 
+.. |CodeQL| image:: https://github.com/thombashi/subprocrunner/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/subprocrunner/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
 
 Usage
 ========
 Execute a command
 ----------------------------
 :Sample Code:
     .. code:: python
@@ -91,15 +105,15 @@
         return code: 0
         stdout: test
         
         SubprocessRunner(command='ls __not_exist_dir__', returncode='not yet executed')
         return code: 2
         stderr: ls: cannot access '__not_exist_dir__': No such file or directory
 
-Execute a command with retry
+Execute a command with retries
 --------------------------------------------------------
 
 :Sample Code:
     .. code:: python
 
         from subprocrunner import Retry, SubprocessRunner
 
@@ -211,16 +225,14 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-subprocrunner
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/subprocrunner/network/dependencies>`__
 
 Optional dependencies
 ----------------------------------
 - `loguru <https://github.com/Delgan/loguru>`__
     - Used for logging if the package installed
-
-
```

### Comparing `subprocrunner-2.0.0/README.rst` & `subprocrunner-2.0.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,40 @@
    :depth: 2
 
 
 Summary
 =============
 A Python wrapper library for ``subprocess`` module.
 
-.. image:: https://badge.fury.io/py/subprocrunner.svg
+|PyPI pkg ver| |Supported Python versions| |Supported Python implementations| |CI status| |Test coverage| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/subprocrunner.svg
     :target: https://badge.fury.io/py/subprocrunner
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/subprocrunner.svg
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/subprocrunner.svg
     :target: https://pypi.org/project/subprocrunner
     :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/implementation/subprocrunner.svg
+.. |Supported Python implementations| image:: https://img.shields.io/pypi/implementation/subprocrunner.svg
     :target: https://pypi.org/project/subprocrunner
     :alt: Supported Python implementations
 
-.. image:: https://github.com/thombashi/subprocrunner/actions/workflows/lint_and_test.yml/badge.svg
-    :target: https://github.com/thombashi/subprocrunner/actions/workflows/lint_and_test.yml
+.. |CI status| image:: https://github.com/thombashi/subprocrunner/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/subprocrunner/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://coveralls.io/repos/github/thombashi/subprocrunner/badge.svg?branch=master
+.. |Test coverage| image:: https://coveralls.io/repos/github/thombashi/subprocrunner/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/subprocrunner?branch=master
     :alt: Test coverage
 
+.. |CodeQL| image:: https://github.com/thombashi/subprocrunner/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/subprocrunner/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
 
 Usage
 ========
 Execute a command
 ----------------------------
 :Sample Code:
     .. code:: python
@@ -54,15 +60,15 @@
         return code: 0
         stdout: test
         
         SubprocessRunner(command='ls __not_exist_dir__', returncode='not yet executed')
         return code: 2
         stderr: ls: cannot access '__not_exist_dir__': No such file or directory
 
-Execute a command with retry
+Execute a command with retries
 --------------------------------------------------------
 
 :Sample Code:
     .. code:: python
 
         from subprocrunner import Retry, SubprocessRunner
 
@@ -174,14 +180,14 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-subprocrunner
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/subprocrunner/network/dependencies>`__
 
 Optional dependencies
 ----------------------------------
 - `loguru <https://github.com/Delgan/loguru>`__
     - Used for logging if the package installed
```

### Comparing `subprocrunner-2.0.0/setup.py` & `subprocrunner-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "subprocrunner"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -51,36 +51,42 @@
     keywords=["library", "subprocess"],
     license=pkg_info["__license__"],
     long_description=long_description,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
+        "Changlog": f"{REPOSITORY_URL:s}/releases",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=install_requires,
-    extras_require={"logging": LOGGING_REQUIRES, "test": tests_requires + LOGGING_REQUIRES},
+    extras_require={
+        "logging": LOGGING_REQUIRES,
+        "test": tests_requires + LOGGING_REQUIRES,
+    },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
+        "Typing :: Typed",
     ],
     cmdclass=get_release_command_class(),
 )
```

### Comparing `subprocrunner-2.0.0/subprocrunner/_logger/_logger.py` & `subprocrunner-2.0.1/subprocrunner/_logger/_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-
 from typing import Callable, Optional
 
 from ._null_logger import NullLogger
 
 
 MODULE_NAME = "subprocrunner"
 DEFAULT_ERROR_LOG_LEVEL = "WARNING"
@@ -15,15 +14,15 @@
 try:
     from loguru import logger
 
     LOGURU_INSTALLED = True
     logger.disable(MODULE_NAME)
 except ImportError:
     LOGURU_INSTALLED = False
-    logger = NullLogger()  # type: ignore
+    logger = NullLogger()
 
 
 def get_logging_method(log_level: Optional[str] = None) -> Callable:
     if not LOGURU_INSTALLED:
         return logger.debug
 
     if log_level is None:
@@ -51,10 +50,10 @@
 def set_logger(is_enable: bool, propagation_depth: int = 1) -> None:
     if is_enable:
         logger.enable(MODULE_NAME)
     else:
         logger.disable(MODULE_NAME)
 
 
-def set_log_level(log_level):
+def set_log_level(log_level):  # type: ignore
     # deprecated
     return
```

### Comparing `subprocrunner-2.0.0/subprocrunner/_logger/_null_logger.py` & `subprocrunner-2.0.1/subprocrunner/_logger/_null_logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# type: ignore
+
+
 class NullLogger:
     level_name = None
 
     def remove(self, handler_id=None):  # pragma: no cover
         pass
 
     def add(self, sink, **kwargs):  # pragma: no cover
```

### Comparing `subprocrunner-2.0.0/subprocrunner/_subprocess_runner.py` & `subprocrunner-2.0.1/subprocrunner/_subprocess_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-
 import errno
 import os
 import platform
 import subprocess
 import traceback
 from subprocess import PIPE
-from typing import Dict, List, Optional, Pattern, Sequence, Union, cast  # noqa
+from typing import Any, Dict, List, Optional, Pattern, Sequence, Union, cast
 
 from mbstrdecoder import MultiByteStrDecoder
 
 from ._logger import DEFAULT_ERROR_LOG_LEVEL, get_logging_method
 from ._which import Which
 from .error import CalledProcessError, CommandError
 from .retry import Retry
 from .typing import Command
 
 
+Env = Dict[str, str]
+
+
 class SubprocessRunner:
     """
     .. py:attribute:: default_is_dry_run
 
         Class wide dry-run setting default value.
         dry-run if ``True``.
 
@@ -129,29 +131,29 @@
         return self.__stderr
 
     @property
     def returncode(self) -> Optional[int]:
         return self.__returncode
 
     @property
-    def error_log_level(self):
+    def error_log_level(self) -> None:
         raise NotImplementedError()
 
     @error_log_level.setter
-    def error_log_level(self, log_level: Optional[str]):
+    def error_log_level(self, log_level: Optional[str]) -> None:
         self.__error_logging_method = get_logging_method(log_level)
 
     def _run(
         self,
-        env,
+        env: Optional[Env],
         check: bool,
         input: Union[str, bytes, None] = None,
         encoding: str = "ascii",
         timeout: Optional[float] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> int:
         self.__save_command()
         self.__debug_print_command(retry_attept=kwargs.get(self._RETRY_ATTEMPT_KEY))
 
         if self._RETRY_ATTEMPT_KEY in kwargs:
             kwargs.pop(self._RETRY_ATTEMPT_KEY)
 
@@ -162,18 +164,22 @@
                 env=env,
                 stdin=PIPE,
                 stdout=PIPE,
                 stderr=PIPE,
             )
         except TypeError:
             proc = subprocess.Popen(
-                self.command, shell=self.__is_shell, stdin=PIPE, stdout=PIPE, stderr=PIPE
+                self.command,
+                shell=self.__is_shell,
+                stdin=PIPE,
+                stdout=PIPE,
+                stderr=PIPE,
             )
 
-        if input and not isinstance(input, bytes) and encoding:
+        if input and isinstance(input, str) and encoding:
             input = input.encode(encoding)
         stdout, stderr = proc.communicate(input=input, timeout=timeout)  # type: ignore
         self.__returncode = proc.returncode
 
         self.__stdout = MultiByteStrDecoder(stdout).unicode_str
         self.__stderr = MultiByteStrDecoder(stderr).unicode_str
 
@@ -201,16 +207,16 @@
         return self.__returncode
 
     def run(
         self,
         input: Union[str, bytes, None] = None,
         encoding: Optional[str] = None,
         timeout: Optional[float] = None,
-        retry: Retry = None,
-        **kwargs,
+        retry: Optional[Retry] = None,
+        **kwargs: Any,
     ) -> int:
         self.__verify_command()
 
         if self.dry_run:
             self.__stdout = self._DRY_RUN_OUTPUT
             self.__stderr = self._DRY_RUN_OUTPUT
             self.__returncode = 0
@@ -240,49 +246,63 @@
                 attempt=i + 1,
                 logging_method=self.__debug_logging_method,
                 retry_target=self.command_str,
             )
             kwargs[self._RETRY_ATTEMPT_KEY] = i + 1
 
             returncode = self._run(
-                env=env, check=False, input=input, encoding=encoding, timeout=timeout, **kwargs
+                env=env,
+                check=False,
+                input=input,
+                encoding=encoding,
+                timeout=timeout,
+                **kwargs,
             )
             if returncode in [0] + retry.no_retry_returncodes:
                 return returncode
 
         if check is True:
             self.raise_for_returncode()
 
         return self.__returncode  # type: ignore
 
-    def popen(self, std_in: Optional[int] = None, env: Optional[Dict[str, str]] = None):
+    def popen(
+        self, std_in: Optional[int] = None, env: Optional[Env] = None
+    ) -> Union[subprocess.Popen, subprocess.CompletedProcess]:
         self.__verify_command()
         self.__debug_print_command()
 
         if self.dry_run:
             self.__stdout = self._DRY_RUN_OUTPUT
             self.__stderr = self._DRY_RUN_OUTPUT
             self.__returncode = 0
 
             return subprocess.CompletedProcess(
-                args=[], returncode=self.__returncode, stdout=self.__stdout, stderr=self.__stderr
+                args=[],
+                returncode=self.__returncode,
+                stdout=self.__stdout,
+                stderr=self.__stderr,
             )
 
         try:
             process = subprocess.Popen(
                 self.command,
                 env=self.__get_env(env),
                 shell=self.__is_shell,
                 stdin=std_in,
                 stdout=PIPE,
                 stderr=PIPE,
             )
         except TypeError:
             process = subprocess.Popen(
-                self.command, shell=self.__is_shell, stdin=std_in, stdout=PIPE, stderr=PIPE
+                self.command,
+                shell=self.__is_shell,
+                stdin=std_in,
+                stdout=PIPE,
+                stderr=PIPE,
             )
 
         return process
 
     def raise_for_returncode(self) -> None:
         if self.__returncode in [None, 0]:
             return
@@ -295,15 +315,17 @@
             output=self.stdout,
             stderr=self.stderr,
         )
 
     def __verify_command(self) -> None:
         if not self.command:
             raise CommandError(
-                f"invalid command: {self.command}", cmd=self.command_str, errno=errno.EINVAL
+                f"invalid command: {self.command}",
+                cmd=self.command_str,
+                errno=errno.EINVAL,
             )
 
         if self.dry_run or platform.system() == "Windows":
             return
 
         if self.__is_shell:
             base_command = cast(str, self.command).split()[0].lstrip("(")
@@ -318,22 +340,22 @@
 
         if len(self.__command_history) >= self.history_size:
             self.__command_history.pop(0)
 
         self.__command_history.append(self.command_str)
 
     @staticmethod
-    def __get_env(env=None):
+    def __get_env(env: Optional[Env] = None) -> Env:
         if env is not None:
             return env
 
         if platform.system() == "Linux":
             return dict(os.environ, LC_ALL="C")
 
-        return os.environ
+        return cast(Env, os.environ)
 
     def __debug_print_command(self, retry_attept: Optional[int] = None) -> None:
         if self.__quiet:
             return
 
         message_list = []
```

### Comparing `subprocrunner-2.0.0/subprocrunner/_which.py` & `subprocrunner-2.0.1/subprocrunner/_which.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,17 @@
 
     def is_exist(self) -> bool:
         return self.abspath() is not None and os.path.exists(str(self.abspath()))
 
     def verify(self) -> None:
         if not self.is_exist():
             raise CommandError(
-                f"command not found: {self.command}", cmd=self.command, errno=errno.ENOENT
+                f"command not found: {self.command}",
+                cmd=self.command,
+                errno=errno.ENOENT,
             )
 
     def abspath(self) -> Optional[str]:
         if self.__abspath:
             return self.__abspath
 
         self.__abspath = shutil.which(self.command)  # type: ignore
```

### Comparing `subprocrunner-2.0.0/subprocrunner/error.py` & `subprocrunner-2.0.1/subprocrunner/error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-
 # keep the following line for backward compatibility
 from subprocess import CalledProcessError  # noqa
-from typing import Optional
+from typing import Any, Optional
 
 from .typing import Command
 
 
 class CommandError(Exception):
     @property
     def cmd(self) -> Optional[Command]:
         return self.__cmd
 
     @property
     def errno(self) -> Optional[int]:
         return self.__errno
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args: str, **kwargs: Any) -> None:
         self.__cmd = kwargs.pop("cmd", None)
         self.__errno = kwargs.pop("errno", None)
 
         super().__init__(*args)
```

### Comparing `subprocrunner-2.0.0/subprocrunner/retry.py` & `subprocrunner-2.0.1/subprocrunner/retry.py`

 * *Files identical despite different names*

### Comparing `subprocrunner-2.0.0/subprocrunner.egg-info/PKG-INFO` & `subprocrunner-2.0.1/subprocrunner.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,87 @@
 Metadata-Version: 2.1
 Name: subprocrunner
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python wrapper library for subprocess module.
 Home-page: https://github.com/thombashi/subprocrunner
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changlog, https://github.com/thombashi/subprocrunner/releases
 Project-URL: Source, https://github.com/thombashi/subprocrunner
 Project-URL: Tracker, https://github.com/thombashi/subprocrunner/issues
 Keywords: library,subprocess
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: mbstrdecoder<2,>=1.0.0
 Provides-Extra: logging
+Requires-Dist: loguru<1,>=0.4.1; extra == "logging"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+Requires-Dist: typepy; extra == "test"
+Requires-Dist: loguru<1,>=0.4.1; extra == "test"
 
 .. contents:: **subprocrunner**
    :backlinks: top
    :depth: 2
 
 
 Summary
 =============
 A Python wrapper library for ``subprocess`` module.
 
-.. image:: https://badge.fury.io/py/subprocrunner.svg
+|PyPI pkg ver| |Supported Python versions| |Supported Python implementations| |CI status| |Test coverage| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/subprocrunner.svg
     :target: https://badge.fury.io/py/subprocrunner
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/subprocrunner.svg
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/subprocrunner.svg
     :target: https://pypi.org/project/subprocrunner
     :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/implementation/subprocrunner.svg
+.. |Supported Python implementations| image:: https://img.shields.io/pypi/implementation/subprocrunner.svg
     :target: https://pypi.org/project/subprocrunner
     :alt: Supported Python implementations
 
-.. image:: https://github.com/thombashi/subprocrunner/actions/workflows/lint_and_test.yml/badge.svg
-    :target: https://github.com/thombashi/subprocrunner/actions/workflows/lint_and_test.yml
+.. |CI status| image:: https://github.com/thombashi/subprocrunner/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/subprocrunner/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://coveralls.io/repos/github/thombashi/subprocrunner/badge.svg?branch=master
+.. |Test coverage| image:: https://coveralls.io/repos/github/thombashi/subprocrunner/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/subprocrunner?branch=master
     :alt: Test coverage
 
+.. |CodeQL| image:: https://github.com/thombashi/subprocrunner/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/subprocrunner/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
 
 Usage
 ========
 Execute a command
 ----------------------------
 :Sample Code:
     .. code:: python
@@ -91,15 +105,15 @@
         return code: 0
         stdout: test
         
         SubprocessRunner(command='ls __not_exist_dir__', returncode='not yet executed')
         return code: 2
         stderr: ls: cannot access '__not_exist_dir__': No such file or directory
 
-Execute a command with retry
+Execute a command with retries
 --------------------------------------------------------
 
 :Sample Code:
     .. code:: python
 
         from subprocrunner import Retry, SubprocessRunner
 
@@ -211,16 +225,14 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-subprocrunner
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/subprocrunner/network/dependencies>`__
 
 Optional dependencies
 ----------------------------------
 - `loguru <https://github.com/Delgan/loguru>`__
     - Used for logging if the package installed
-
-
```

### Comparing `subprocrunner-2.0.0/subprocrunner.egg-info/SOURCES.txt` & `subprocrunner-2.0.1/subprocrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subprocrunner-2.0.0/test/test_logger.py` & `subprocrunner-2.0.1/test/test_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-
 import pytest
 
 from subprocrunner import set_logger
 from subprocrunner._logger._null_logger import NullLogger
 
 
 class Test_set_logger:
```

### Comparing `subprocrunner-2.0.0/test/test_retry.py` & `subprocrunner-2.0.1/test/test_retry.py`

 * *Files identical despite different names*

### Comparing `subprocrunner-2.0.0/test/test_subproc_runner.py` & `subprocrunner-2.0.1/test/test_subproc_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-
 import errno
 import os
 import platform
 import re
+import subprocess
 import sys
 from subprocess import PIPE
 
 import pytest
 from typepy import is_not_null_string, is_null_string
 
 from subprocrunner import SubprocessRunner
@@ -96,14 +96,15 @@
     def test_stdout(self, command, expected):
         runner = SubprocessRunner(command)
         runner.run()
 
         assert runner.command == command
         assert isinstance(runner.command_str, str)
         assert runner.returncode == 0
+        assert runner.stdout
         assert runner.stdout.strip() == expected
         assert is_null_string(runner.stderr)
 
     @pytest.mark.skip
     @pytest.mark.parametrize(
         ["command", "ignore_stderr_regexp", "out_regexp", "expected"],
         [
@@ -125,14 +126,16 @@
         logger.add(sys.stderr, level="DEBUG")
         logger.enable("test")
         subprocrunner.set_logger(True)
 
         runner = SubprocessRunner(command, ignore_stderr_regexp=ignore_stderr_regexp)
         runner.run()
 
+        assert runner.stdout
+        assert runner.stderr
         assert is_null_string(runner.stdout.strip())
         assert is_not_null_string(runner.stderr.strip())
         assert runner.returncode != 0
 
         out, err = capsys.readouterr()
         print(f"[sys stdout]\n{out}\n")
         print(f"[sys stderr]\n{err}\n")
@@ -143,15 +146,19 @@
         assert actual == expected
 
     @pytest.mark.skipif(platform.system() == "Windows", reason="platform dependent tests")
     @pytest.mark.parametrize(
         ["command", "ignore_stderr_regexp", "expected"],
         [
             [[list_command, "__not_exist_dir__"], None, CalledProcessError],
-            [[list_command, "__not_exist_dir__"], re.compile(re.escape("__not_exist_dir__")), None],
+            [
+                [list_command, "__not_exist_dir__"],
+                re.compile(re.escape("__not_exist_dir__")),
+                None,
+            ],
         ],
     )
     def test_stderr_check(self, command, ignore_stderr_regexp, expected):
         runner = SubprocessRunner(command, ignore_stderr_regexp=ignore_stderr_regexp)
 
         if ignore_stderr_regexp:
             runner.run(check=True)
@@ -178,15 +185,16 @@
 
         mocked_communicate.assert_called_with(input=None, timeout=1)
 
     def test_unicode(self, mocker):
         mocked_communicate = mocker.patch("subprocess.Popen.communicate")
         mocked_communicate.return_value = (
             "",
-            "'dummy' は、内部コマンドまたは外部コマンド、" "操作可能なプログラムまたはバッチ ファイルとして認識されていません",
+            "'dummy' は、内部コマンドまたは外部コマンド、"
+            "操作可能なプログラムまたはバッチ ファイルとして認識されていません",
         )
 
         runner = SubprocessRunner(list_command)
         runner.run()
 
     def test_retry(self, mocker):
         mocker.patch("subprocrunner.Which.verify")
@@ -256,34 +264,42 @@
                 return 1
 
             return 0
 
         runner = SubprocessRunner("always-failed-command")
         mocked_run = mocker.patch("subprocrunner.SubprocessRunner._run")
         mocked_run.side_effect = failed_first_call
-        runner.run(check=True, retry=Retry(total=3, backoff_factor=BACKOFF_FACTOR, jitter=JITTER))
+        runner.run(
+            check=True,
+            retry=Retry(total=3, backoff_factor=BACKOFF_FACTOR, jitter=JITTER),
+        )
         assert mocked_run.call_count == 2
 
 
 class Test_SubprocessRunner_popen:
     @pytest.mark.parametrize(
         ["command", "environ", "expected"],
-        [["hostname", None, 0], ["hostname", dict(os.environ), 0]],
+        [
+            ["hostname", None, 0],
+            ["hostname", dict(os.environ), 0],
+        ],
     )
     def test_normal(self, command, environ, expected):
         proc = SubprocessRunner(command).popen(env=environ)
+        assert isinstance(proc, subprocess.Popen)
         ret_stdout, ret_stderr = proc.communicate()
         assert is_not_null_string(ret_stdout)
         assert is_null_string(ret_stderr)
         assert proc.returncode == expected
 
     @pytest.mark.skipif(platform.system() == "Windows", reason="platform dependent tests")
     @pytest.mark.parametrize(["command", "pipe_input", "expected"], [["grep a", b"aaa", 0]])
     def test_normal_stdin(self, command, pipe_input, expected):
         proc = SubprocessRunner(command).popen(PIPE)
+        assert isinstance(proc, subprocess.Popen)
         ret_stdout, ret_stderr = proc.communicate(input=pipe_input)
 
         assert is_not_null_string(ret_stdout)
         assert is_null_string(ret_stderr)
         assert proc.returncode == expected
```

### Comparing `subprocrunner-2.0.0/test/test_which.py` & `subprocrunner-2.0.1/test/test_which.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-
 import platform
 import re
 import sys
 
 import pytest
 from typepy import is_not_null_string
 
@@ -50,15 +49,20 @@
         print(actual, file=sys.stderr)
         assert expected_regexp.search(actual) is not None
 
 
 class Test_Which_is_exist:
     @pytest.mark.skipif(platform.system() == "Windows", reason="platform dependent tests")
     @pytest.mark.parametrize(
-        ["value", "expected"], [["ls", True], ["/bin/ls", True], ["__not_exist_command__", False]]
+        ["value", "expected"],
+        [
+            ["ls", True],
+            ["/bin/ls", True],
+            ["__not_exist_command__", False],
+        ],
     )
     def test_normal_linux(self, value, expected):
         assert Which(value).is_exist() == expected
 
     @pytest.mark.skipif(platform.system() != "Windows", reason="platform dependent tests")
     @pytest.mark.parametrize(
         ["value", "expected"], [["ping", True], ["__not_exist_command__", False]]
```

### Comparing `subprocrunner-2.0.0/tox.ini` & `subprocrunner-2.0.1/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,79 @@
 [tox]
 envlist =
-    py{36,37,38,39,310}
+    py{37,38,39,310,311,312}
     pypy3
     build
-    clean
     cov
     fmt
     lint
 
 [testenv]
-deps =
-    .[test]
+extras =
+    test
 commands =
     pytest {posargs}
 
 [testenv:build]
-basepython = python3.8
 deps =
+    build>=1
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*.whl dist/*.tar.gz
-    python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
-    cleanpy>=0.3.1
+    cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
 [testenv:cov]
+extras =
+    test
 deps =
-    .[test]
     coverage[toml]
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
-[testenv:fmt]
-basepython = python3.8
+[testenv:fmt-black]
 skip_install = true
 deps =
-    autoflake
-    black[jupyter]
+    autoflake>=2
+    black[jupyter]>=24.1
     isort>=5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
     isort .
     black setup.py examples test subprocrunner
 
-[testenv:lint]
-basepython = python3.8
+[testenv:fmt]
 skip_install = true
 deps =
-    codespell
-    mypy>=0.910
-    pylama>=8.3.6
+    autoflake>=2
+    isort>=5
+    ruff>=0.3.5
+commands =
+    autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
+    isort .
+    ruff format setup.py examples test subprocrunner
+
+[testenv:lint]
+extras =
+    test
+deps =
+    codespell>=2
+    mypy>=1
+    ; pylama>=8.4.1
+    pyright>=1.1
+    releasecmd
+    ruff>=0.3.5
 commands =
-    python setup.py check
-    mypy subprocrunner
+    ; mypy subprocrunner
+    pyright
     codespell subprocrunner examples test README.rst -q 2 --check-filenames
-    pylama
+    ; pylama
+    ruff format --check
+    ruff check
```

