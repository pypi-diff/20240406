# Comparing `tmp/datasette-paste-0.1a4.tar.gz` & `tmp/datasette-paste-0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-paste-0.1a4.tar", last modified: Fri Mar 29 21:31:12 2024, max compression
+gzip compressed data, was "datasette-paste-0.1a5.tar", last modified: Sat Apr  6 16:25:56 2024, max compression
```

## Comparing `datasette-paste-0.1a4.tar` & `datasette-paste-0.1a5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:31:12.554097 datasette-paste-0.1a4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-29 21:31:06.000000 datasette-paste-0.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-29 21:31:12.554097 datasette-paste-0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-29 21:31:06.000000 datasette-paste-0.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:31:12.554097 datasette-paste-0.1a4/datasette_paste/
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-29 21:31:06.000000 datasette-paste-0.1a4/datasette_paste/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:31:12.554097 datasette-paste-0.1a4/datasette_paste/static/
--rw-r--r--   0 runner    (1001) docker     (127)    19469 2024-03-29 21:31:06.000000 datasette-paste-0.1a4/datasette_paste/static/papaparse-5-4-1.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:31:12.554097 datasette-paste-0.1a4/datasette_paste/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-03-29 21:31:06.000000 datasette-paste-0.1a4/datasette_paste/templates/paste_create_table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:31:12.554097 datasette-paste-0.1a4/datasette_paste.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-29 21:31:12.000000 datasette-paste-0.1a4/datasette_paste.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-29 21:31:12.000000 datasette-paste-0.1a4/datasette_paste.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 21:31:12.000000 datasette-paste-0.1a4/datasette_paste.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-29 21:31:12.000000 datasette-paste-0.1a4/datasette_paste.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-29 21:31:12.000000 datasette-paste-0.1a4/datasette_paste.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 21:31:12.000000 datasette-paste-0.1a4/datasette_paste.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-29 21:31:06.000000 datasette-paste-0.1a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 21:31:12.554097 datasette-paste-0.1a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:31:12.554097 datasette-paste-0.1a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-29 21:31:06.000000 datasette-paste-0.1a4/tests/test_paste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:25:56.021355 datasette-paste-0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 16:25:50.000000 datasette-paste-0.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-06 16:25:56.021355 datasette-paste-0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-06 16:25:50.000000 datasette-paste-0.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:25:56.021355 datasette-paste-0.1a5/datasette_paste/
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-06 16:25:50.000000 datasette-paste-0.1a5/datasette_paste/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:25:56.021355 datasette-paste-0.1a5/datasette_paste/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    19469 2024-04-06 16:25:50.000000 datasette-paste-0.1a5/datasette_paste/static/papaparse-5-4-1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:25:56.021355 datasette-paste-0.1a5/datasette_paste/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-06 16:25:50.000000 datasette-paste-0.1a5/datasette_paste/templates/paste_create_table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:25:56.021355 datasette-paste-0.1a5/datasette_paste.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-06 16:25:56.000000 datasette-paste-0.1a5/datasette_paste.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-06 16:25:56.000000 datasette-paste-0.1a5/datasette_paste.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:25:56.000000 datasette-paste-0.1a5/datasette_paste.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 16:25:56.000000 datasette-paste-0.1a5/datasette_paste.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-06 16:25:56.000000 datasette-paste-0.1a5/datasette_paste.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 16:25:56.000000 datasette-paste-0.1a5/datasette_paste.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-06 16:25:50.000000 datasette-paste-0.1a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:25:56.021355 datasette-paste-0.1a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:25:56.021355 datasette-paste-0.1a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-06 16:25:50.000000 datasette-paste-0.1a5/tests/test_paste.py
```

### Comparing `datasette-paste-0.1a4/LICENSE` & `datasette-paste-0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-paste-0.1a4/PKG-INFO` & `datasette-paste-0.1a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-paste
-Version: 0.1a4
+Version: 0.1a5
 Summary: Paste data to create tables in Datasette
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-paste
 Project-URL: Changelog, https://github.com/datasette/datasette-paste/releases
 Project-URL: Issues, https://github.com/datasette/datasette-paste/issues
 Project-URL: CI, https://github.com/datasette/datasette-paste/actions
@@ -23,14 +23,16 @@
 [![PyPI](https://img.shields.io/pypi/v/datasette-paste.svg)](https://pypi.org/project/datasette-paste/)
 [![Changelog](https://img.shields.io/github/v/release/datasette/datasette-paste?include_prereleases&label=changelog)](https://github.com/datasette/datasette-paste/releases)
 [![Tests](https://github.com/datasette/datasette-paste/actions/workflows/test.yml/badge.svg)](https://github.com/datasette/datasette-paste/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-paste/blob/main/LICENSE)
 
 Paste data to create tables in Datasette
 
+**This plugin is no longer being developed.** It has been replaced by [datasette-import](https://github.com/datasette/datasette-import).
+
 ## Installation
 
 Install this plugin in the same environment as Datasette.
 ```bash
 datasette install datasette-paste
 ```
 ## Usage
```

### Comparing `datasette-paste-0.1a4/README.md` & `datasette-paste-0.1a5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 [![PyPI](https://img.shields.io/pypi/v/datasette-paste.svg)](https://pypi.org/project/datasette-paste/)
 [![Changelog](https://img.shields.io/github/v/release/datasette/datasette-paste?include_prereleases&label=changelog)](https://github.com/datasette/datasette-paste/releases)
 [![Tests](https://github.com/datasette/datasette-paste/actions/workflows/test.yml/badge.svg)](https://github.com/datasette/datasette-paste/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-paste/blob/main/LICENSE)
 
 Paste data to create tables in Datasette
 
+**This plugin is no longer being developed.** It has been replaced by [datasette-import](https://github.com/datasette/datasette-import).
+
 ## Installation
 
 Install this plugin in the same environment as Datasette.
 ```bash
 datasette install datasette-paste
 ```
 ## Usage
```

### Comparing `datasette-paste-0.1a4/datasette_paste/__init__.py` & `datasette-paste-0.1a5/datasette_paste/__init__.py`

 * *Files identical despite different names*

### Comparing `datasette-paste-0.1a4/datasette_paste/static/papaparse-5-4-1.min.js` & `datasette-paste-0.1a5/datasette_paste/static/papaparse-5-4-1.min.js`

 * *Files identical despite different names*

### Comparing `datasette-paste-0.1a4/datasette_paste/templates/paste_create_table.html` & `datasette-paste-0.1a5/datasette_paste/templates/paste_create_table.html`

 * *Files identical despite different names*

### Comparing `datasette-paste-0.1a4/datasette_paste.egg-info/PKG-INFO` & `datasette-paste-0.1a5/datasette_paste.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-paste
-Version: 0.1a4
+Version: 0.1a5
 Summary: Paste data to create tables in Datasette
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-paste
 Project-URL: Changelog, https://github.com/datasette/datasette-paste/releases
 Project-URL: Issues, https://github.com/datasette/datasette-paste/issues
 Project-URL: CI, https://github.com/datasette/datasette-paste/actions
@@ -23,14 +23,16 @@
 [![PyPI](https://img.shields.io/pypi/v/datasette-paste.svg)](https://pypi.org/project/datasette-paste/)
 [![Changelog](https://img.shields.io/github/v/release/datasette/datasette-paste?include_prereleases&label=changelog)](https://github.com/datasette/datasette-paste/releases)
 [![Tests](https://github.com/datasette/datasette-paste/actions/workflows/test.yml/badge.svg)](https://github.com/datasette/datasette-paste/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-paste/blob/main/LICENSE)
 
 Paste data to create tables in Datasette
 
+**This plugin is no longer being developed.** It has been replaced by [datasette-import](https://github.com/datasette/datasette-import).
+
 ## Installation
 
 Install this plugin in the same environment as Datasette.
 ```bash
 datasette install datasette-paste
 ```
 ## Usage
```

### Comparing `datasette-paste-0.1a4/pyproject.toml` & `datasette-paste-0.1a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-paste"
-version = "0.1a4"
+version = "0.1a5"
 description = "Paste data to create tables in Datasette"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `datasette-paste-0.1a4/tests/test_paste.py` & `datasette-paste-0.1a5/tests/test_paste.py`

 * *Files identical despite different names*

