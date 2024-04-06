# Comparing `tmp/pytest-data-suites-1.0.4.tar.gz` & `tmp/pytest_data_suites-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-data-suites-1.0.4.tar", max compression
+gzip compressed data, was "pytest_data_suites-1.0.5.tar", max compression
```

## Comparing `pytest-data-suites-1.0.4.tar` & `pytest_data_suites-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1057 2022-06-18 11:35:40.786525 pytest-data-suites-1.0.4/LICENSE
--rw-r--r--   0        0        0      698 2022-06-19 08:08:41.219156 pytest-data-suites-1.0.4/README.md
--rw-r--r--   0        0        0      906 2022-07-24 06:52:47.926390 pytest-data-suites-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      135 2022-07-24 06:52:41.370367 pytest-data-suites-1.0.4/src/pytest_data_suites/__init__.py
--rw-r--r--   0        0        0        0 2022-06-18 21:59:26.709750 pytest-data-suites-1.0.4/src/pytest_data_suites/py.typed
--rw-r--r--   0        0        0     3488 2022-07-24 06:52:41.355271 pytest-data-suites-1.0.4/src/pytest_data_suites/suite.py
--rw-r--r--   0        0        0      657 2022-06-18 11:36:37.998924 pytest-data-suites-1.0.4/src/pytest_data_suites/utils.py
--rw-r--r--   0        0        0      328 2022-06-18 20:43:14.148721 pytest-data-suites-1.0.4/src/pytest_data_suites/version.py
--rw-r--r--   0        0        0     1471 2022-07-24 06:55:02.246784 pytest-data-suites-1.0.4/setup.py
--rw-r--r--   0        0        0     1490 2022-07-24 06:55:02.247052 pytest-data-suites-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-04-06 13:35:02.937454 pytest_data_suites-1.0.5/LICENSE
+-rw-r--r--   0        0        0      698 2024-04-06 13:35:02.937651 pytest_data_suites-1.0.5/README.md
+-rw-r--r--   0        0        0      925 2024-04-06 14:05:46.743023 pytest_data_suites-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      135 2024-04-06 13:35:02.938819 pytest_data_suites-1.0.5/src/pytest_data_suites/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 13:35:02.938956 pytest_data_suites-1.0.5/src/pytest_data_suites/py.typed
+-rw-r--r--   0        0        0     3488 2024-04-06 13:35:02.939159 pytest_data_suites-1.0.5/src/pytest_data_suites/suite.py
+-rw-r--r--   0        0        0      657 2024-04-06 13:35:02.939349 pytest_data_suites-1.0.5/src/pytest_data_suites/utils.py
+-rw-r--r--   0        0        0      328 2024-04-06 13:35:02.939537 pytest_data_suites-1.0.5/src/pytest_data_suites/version.py
+-rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 pytest_data_suites-1.0.5/PKG-INFO
```

### Comparing `pytest-data-suites-1.0.4/LICENSE` & `pytest_data_suites-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-data-suites-1.0.4/README.md` & `pytest_data_suites-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pytest-data-suites-1.0.4/pyproject.toml` & `pytest_data_suites-1.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-data-suites"
-version = "1.0.4"
+version = "1.0.5"
 description = "Class-based pytest parametrization"
 license = "MIT"
 authors = [
     "Artem Novikov <artnew@list.ru>",
 ]
 readme = "README.md"
 repository = "https://github.com/reartnew/pytest-data-suites"
@@ -12,25 +12,25 @@
     "Topic :: Software Development :: Testing",
     "Framework :: Pytest",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pytest = "^6.0 || ^7.0"
-coverage = "*"
+pytest = ">=6.0, <9.0"
 
-[tool.poetry.dev-dependencies]
-pytest-pylint = "*"
-pylint-quotes = "*"
-pytest-ordering = "*"
-pytest-mypy = "*"
-pytest-black = "*"
-pytest-bandit = "*"
-tox-poetry-dev-dependencies = "*"
+[tool.poetry.group.dev.dependencies]
+pylint = "^3.1.0"
+pytest-pylint = "^0.21.0"
+pytest-ordering = "^0.6"
+pytest-mypy = "^0.10.3"
+pytest-black = "^0.3.12"
+pytest-bandit = "^0.6.1"
+tox = "^4.14.2"
+setuptools = "^69.2.0"
 
 [tool.pytest.ini_options]
 testpaths = [
     "src",
     "tests",
 ]
 addopts = """
```

### Comparing `pytest-data-suites-1.0.4/src/pytest_data_suites/suite.py` & `pytest_data_suites-1.0.5/src/pytest_data_suites/suite.py`

 * *Files identical despite different names*

### Comparing `pytest-data-suites-1.0.4/src/pytest_data_suites/utils.py` & `pytest_data_suites-1.0.5/src/pytest_data_suites/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-data-suites-1.0.4/PKG-INFO` & `pytest_data_suites-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pytest-data-suites
-Version: 1.0.4
+Version: 1.0.5
 Summary: Class-based pytest parametrization
 Home-page: https://github.com/reartnew/pytest-data-suites
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
-Requires-Dist: coverage
-Requires-Dist: pytest (>=6.0,<8.0)
+Requires-Dist: pytest (>=6.0,<9.0)
 Project-URL: Repository, https://github.com/reartnew/pytest-data-suites
 Description-Content-Type: text/markdown
 
 # pytest-data-suites
 
 Class-based test cases for `pytest`.
```

