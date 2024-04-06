# Comparing `tmp/aoc_core-0.1.2.tar.gz` & `tmp/aoc_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aoc_core-0.1.2.tar", max compression
+gzip compressed data, was "aoc_core-0.1.3.tar", max compression
```

## Comparing `aoc_core-0.1.2.tar` & `aoc_core-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1092 2024-02-26 12:10:59.963886 aoc_core-0.1.2/LICENSE
--rw-r--r--   0        0        0     7799 2024-02-26 12:10:59.963886 aoc_core-0.1.2/README.md
--rw-r--r--   0        0        0     1607 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/__init__.py
--rw-r--r--   0        0        0       92 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/__main__.py
--rw-r--r--   0        0        0     2711 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/constants.py
--rw-r--r--   0        0        0     1898 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/data.py
--rw-r--r--   0        0        0     1241 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/errors.py
--rw-r--r--   0        0        0      107 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/ext/__init__.py
--rw-r--r--   0        0        0      513 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/ext/constants.py
--rw-r--r--   0        0        0     1162 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/ext/splits.py
--rw-r--r--   0        0        0     6919 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/http.py
--rw-r--r--   0        0        0    13633 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/main.py
--rw-r--r--   0        0        0     2417 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/names.py
--rw-r--r--   0        0        0     1842 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/primitives.py
--rw-r--r--   0        0        0     2675 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/runners.py
--rw-r--r--   0        0        0     5463 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/solutions.py
--rw-r--r--   0        0        0     2681 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/states.py
--rw-r--r--   0        0        0      664 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/time.py
--rw-r--r--   0        0        0     2260 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/timers.py
--rw-r--r--   0        0        0     1479 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/tokens.py
--rw-r--r--   0        0        0      289 2024-02-26 12:10:59.963886 aoc_core-0.1.2/aoc/versions.py
--rw-r--r--   0        0        0     3025 2024-02-26 12:10:59.967885 aoc_core-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9423 1970-01-01 00:00:00.000000 aoc_core-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-06 20:24:17.613934 aoc_core-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7799 2024-04-06 20:24:17.613934 aoc_core-0.1.3/README.md
+-rw-r--r--   0        0        0     1607 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/__main__.py
+-rw-r--r--   0        0        0     2711 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/constants.py
+-rw-r--r--   0        0        0     1898 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/data.py
+-rw-r--r--   0        0        0     1241 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/errors.py
+-rw-r--r--   0        0        0      107 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/ext/__init__.py
+-rw-r--r--   0        0        0      513 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/ext/constants.py
+-rw-r--r--   0        0        0     1162 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/ext/splits.py
+-rw-r--r--   0        0        0     6919 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/http.py
+-rw-r--r--   0        0        0    13633 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/main.py
+-rw-r--r--   0        0        0     2575 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/names.py
+-rw-r--r--   0        0        0     1842 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/primitives.py
+-rw-r--r--   0        0        0     2675 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/runners.py
+-rw-r--r--   0        0        0     5463 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/solutions.py
+-rw-r--r--   0        0        0     2681 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/states.py
+-rw-r--r--   0        0        0      664 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/time.py
+-rw-r--r--   0        0        0     2260 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/timers.py
+-rw-r--r--   0        0        0     1479 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/tokens.py
+-rw-r--r--   0        0        0      289 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/versions.py
+-rw-r--r--   0        0        0     2998 2024-04-06 20:24:17.617934 aoc_core-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9423 1970-01-01 00:00:00.000000 aoc_core-0.1.3/PKG-INFO
```

### Comparing `aoc_core-0.1.2/LICENSE` & `aoc_core-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/README.md` & `aoc_core-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add aoc-core
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-aoc-core = "^0.1.2"
+aoc-core = "^0.1.3"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.aoc-core]
 git = "https://github.com/nekitdev/aoc-core.git"
```

### Comparing `aoc_core-0.1.2/aoc/__init__.py` & `aoc_core-0.1.3/aoc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Advent of Code in Python."
 __url__ = "https://github.com/nekitdev/aoc-core"
 
 __title__ = "aoc"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 from aoc.data import dump_data, get_path_for_key, load_data
 from aoc.errors import DataNotFound, InternalError, TokenNotFound
 from aoc.http import HTTPClient, Route
 from aoc.names import get_key_by_name, get_name_by_key
 from aoc.primitives import Day, Key, Year
 from aoc.runners import Results, Runner, run_path
```

### Comparing `aoc_core-0.1.2/aoc/constants.py` & `aoc_core-0.1.3/aoc/constants.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/data.py` & `aoc_core-0.1.3/aoc/data.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/errors.py` & `aoc_core-0.1.3/aoc/errors.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/ext/constants.py` & `aoc_core-0.1.3/aoc/ext/constants.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/ext/splits.py` & `aoc_core-0.1.3/aoc/ext/splits.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/http.py` & `aoc_core-0.1.3/aoc/http.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/main.py` & `aoc_core-0.1.3/aoc/main.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/names.py` & `aoc_core-0.1.3/aoc/names.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,38 +3,45 @@
 
 from aoc.errors import InternalError
 from aoc.primitives import Day, Key, Year
 
 __all__ = ("get_key_by_name", "get_name_by_key")
 
 YEAR: Literal["year"] = "year"
+"""The `year` literal."""
+
 DAY: Literal["day"] = "day"
+"""The `day` literal."""
+
+YEAR_TITLE = YEAR.title()
+"""The `Year` literal."""
+DAY_TITLE = DAY.title()
+"""The `Day` literal."""
 
-NAME_PATTERN = r"^Year(?P<year>[0-9]{4})Day(?P<day>[0-9]{2})$"
+NAME_PATTERN = rf"^{YEAR_TITLE}(?P<{YEAR}>[0-9]{{4}}){DAY_TITLE}(?P<{DAY}>[0-9]{{2}})$"
 
 NAME = compile(NAME_PATTERN)
 
-NAME_EXAMPLE = "YearYYYYDayDD"
-"""The example of the name format."""
+NAME_EXAMPLE = f"{YEAR_TITLE}YYYY{DAY_TITLE}DD"
 
 INVALID_NAME = f"invalid name `{{}}`; expected `{NAME_EXAMPLE}` format"
 invalid_name = INVALID_NAME.format
 
 INVALID_NAME_WITH_REASON = "invalid name `{}` ({})"
 invalid_name_with_reason = INVALID_NAME_WITH_REASON.format
 
-NAME_MATCHED_BUT_NO_YEAR = "name matched but the year group is not set"
-NAME_MATCHED_BUT_NO_DAY = "name matched but the day group is not set"
+NAME_MATCHED_BUT_NO_YEAR = "name matched but the `year` group was not found"
+NAME_MATCHED_BUT_NO_DAY = "name matched but the `day` group was not found"
 
 
 def get_key_by_name(name: str) -> Key:
     """Gets the key representing the problem by the name of the solution type.
 
     Note:
-        The `name` must match the format of [`NAME_EXAMPLE`][aoc.names.NAME_EXAMPLE].
+        The `name` must match the format of `YearYYYYDayDD`.
 
     Arguments:
         name: The name of the solution type.
 
     Returns:
         The key representing the problem.
 
@@ -47,22 +54,22 @@
 
     if match is None:
         raise TypeError(invalid_name(name))
 
     year_option = match.group(YEAR)
 
     if year_option is None:
-        raise InternalError  # TODO: message?
+        raise InternalError(NAME_MATCHED_BUT_NO_YEAR)
 
     year_value = int(year_option)
 
     day_option = match.group(DAY)
 
     if day_option is None:
-        raise InternalError  # TODO: message?
+        raise InternalError(NAME_MATCHED_BUT_NO_DAY)
 
     day_value = int(day_option)
 
     try:
         year = Year(year_value)
 
     except ValueError as invalid_year:
```

### Comparing `aoc_core-0.1.2/aoc/primitives.py` & `aoc_core-0.1.3/aoc/primitives.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/runners.py` & `aoc_core-0.1.3/aoc/runners.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/solutions.py` & `aoc_core-0.1.3/aoc/solutions.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/states.py` & `aoc_core-0.1.3/aoc/states.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/time.py` & `aoc_core-0.1.3/aoc/time.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/timers.py` & `aoc_core-0.1.3/aoc/timers.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/aoc/tokens.py` & `aoc_core-0.1.3/aoc/tokens.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.2/pyproject.toml` & `aoc_core-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aoc-core"
-version = "0.1.2"
+version = "0.1.3"
 description = "Advent of Code in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/aoc-core"
@@ -39,70 +39,69 @@
 
 pendulum = ">= 3.0.0"
 
 click = ">= 8.1.7"
 
 versions = ">= 2.1.2"
 
-entrypoint = ">= 2.0.2"
+entrypoint = ">= 2.0.3"
 
 aiohttp = ">= 3.9.3"
 yarl = ">= 1.9.4"
 
-typing-aliases = ">= 1.7.1"
+typing-aliases = ">= 1.8.0"
 typing-extensions = ">= 4.10.0"
-wraps = ">= 0.9.1"
+wraps = ">= 0.9.2"
 
 [tool.poetry.dependencies.trogon]
 version = ">= 0.5.0"
 python = "^3.8"
 
 [tool.poetry.dependencies.funcs]
-version = ">= 0.9.1"
+version = ">= 0.9.2"
 optional = true
 
 [tool.poetry.dependencies.iters]
-version = ">= 0.16.1"
+version = ">= 0.16.2"
 optional = true
 
 [tool.poetry.extras]
 ext = ["funcs", "iters"]  # `wraps` is required to handle panics
 
 [tool.poetry.group.format.dependencies]
-ruff = "0.2.2"
+ruff = "0.3.3"
 
 [tool.poetry.group.check.dependencies]
-mypy = "1.8.0"
+mypy = "1.9.0"
 
 [tool.poetry.group.check.dependencies.pre-commit]
 version = "3.6.2"
 python = ">= 3.9"
 
 [tool.poetry.group.test.dependencies]
-coverage = "7.4.3"
-pytest = "8.0.2"
+coverage = "7.4.4"
+pytest = "8.1.1"
 pytest-cov = "4.1.0"
-pytest-benchmark = "4.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
-mkdocs-material = "9.5.11"
+mkdocs-material = "9.5.13"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
 version = "0.24.0"
 extras = ["python"]
 
 [tool.poetry.group.release]
 optional = true
 
 [tool.poetry.group.release.dependencies]
-changelogging = "1.4.1"
+changelogging = "1.4.2"
 
 [tool.ruff]
 line-length = 100
 
 [tool.ruff.lint]
 ignore = [
     "E741",  # ambiguous variable name
@@ -132,15 +131,15 @@
 directory = "coverage"
 
 [tool.mypy]
 strict = true
 
 [tool.changelogging]
 name = "aoc-core"
-version = "0.1.2"
+version = "0.1.3"
 url = "https://github.com/nekitdev/aoc-core"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `aoc_core-0.1.2/PKG-INFO` & `aoc_core-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aoc-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: Advent of Code in Python.
 Home-page: https://github.com/nekitdev/aoc-core
 License: MIT
 Keywords: python,aoc
 Author: nekitdev
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
@@ -19,23 +19,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: ext
 Requires-Dist: aiohttp (>=3.9.3)
 Requires-Dist: attrs (>=23.2.0)
 Requires-Dist: click (>=8.1.7)
-Requires-Dist: entrypoint (>=2.0.2)
-Requires-Dist: funcs (>=0.9.1) ; extra == "ext"
-Requires-Dist: iters (>=0.16.1) ; extra == "ext"
+Requires-Dist: entrypoint (>=2.0.3)
+Requires-Dist: funcs (>=0.9.2) ; extra == "ext"
+Requires-Dist: iters (>=0.16.2) ; extra == "ext"
 Requires-Dist: pendulum (>=3.0.0)
 Requires-Dist: trogon (>=0.5.0) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: typing-aliases (>=1.7.1)
+Requires-Dist: typing-aliases (>=1.8.0)
 Requires-Dist: typing-extensions (>=4.10.0)
 Requires-Dist: versions (>=2.1.2)
-Requires-Dist: wraps (>=0.9.1)
+Requires-Dist: wraps (>=0.9.2)
 Requires-Dist: yarl (>=1.9.4)
 Project-URL: Chat, https://nekit.dev/chat
 Project-URL: Documentation, https://nekitdev.github.io/aoc-core
 Project-URL: Funding, https://nekit.dev/funding
 Project-URL: Issues, https://github.com/nekitdev/aoc-core/issues
 Project-URL: Repository, https://github.com/nekitdev/aoc-core
 Description-Content-Type: text/markdown
@@ -82,15 +82,15 @@
 $ poetry add aoc-core
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-aoc-core = "^0.1.2"
+aoc-core = "^0.1.3"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.aoc-core]
 git = "https://github.com/nekitdev/aoc-core.git"
```
