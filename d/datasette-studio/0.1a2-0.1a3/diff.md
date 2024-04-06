# Comparing `tmp/datasette-studio-0.1a2.tar.gz` & `tmp/datasette-studio-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-studio-0.1a2.tar", last modified: Mon Mar 18 17:08:10 2024, max compression
+gzip compressed data, was "datasette-studio-0.1a3.tar", last modified: Sat Apr  6 16:36:43 2024, max compression
```

## Comparing `datasette-studio-0.1a2.tar` & `datasette-studio-0.1a3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:08:10.043096 datasette-studio-0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-18 17:08:04.000000 datasette-studio-0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-18 17:08:10.039096 datasette-studio-0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-18 17:08:04.000000 datasette-studio-0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:08:10.039096 datasette-studio-0.1a2/datasette_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-18 17:08:10.000000 datasette-studio-0.1a2/datasette_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-18 17:08:10.000000 datasette-studio-0.1a2/datasette_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 17:08:10.000000 datasette-studio-0.1a2/datasette_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 17:08:10.000000 datasette-studio-0.1a2/datasette_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-18 17:08:10.000000 datasette-studio-0.1a2/datasette_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 17:08:10.000000 datasette-studio-0.1a2/datasette_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-18 17:08:04.000000 datasette-studio-0.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 17:08:10.043096 datasette-studio-0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:36:43.442007 datasette-studio-0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 16:36:32.000000 datasette-studio-0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-06 16:36:43.442007 datasette-studio-0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-06 16:36:32.000000 datasette-studio-0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:36:43.442007 datasette-studio-0.1a3/datasette_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-06 16:36:43.000000 datasette-studio-0.1a3/datasette_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-06 16:36:43.000000 datasette-studio-0.1a3/datasette_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:36:43.000000 datasette-studio-0.1a3/datasette_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 16:36:43.000000 datasette-studio-0.1a3/datasette_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 16:36:43.000000 datasette-studio-0.1a3/datasette_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:36:43.000000 datasette-studio-0.1a3/datasette_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-06 16:36:32.000000 datasette-studio-0.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:36:43.442007 datasette-studio-0.1a3/setup.cfg
```

### Comparing `datasette-studio-0.1a2/LICENSE` & `datasette-studio-0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-studio-0.1a2/PKG-INFO` & `datasette-studio-0.1a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-studio
-Version: 0.1a2
+Version: 0.1a3
 Summary: Datasette pre-configured with useful plugins
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-studio
 Project-URL: Changelog, https://github.com/datasette/datasette-studio/releases
 Project-URL: Issues, https://github.com/datasette/datasette-studio/issues
 Project-URL: CI, https://github.com/datasette/datasette-studio/actions
@@ -21,26 +21,29 @@
 Requires-Dist: datasette-enrichments
 Requires-Dist: datasette-enrichments-quickjs
 Requires-Dist: datasette-enrichments-re2
 Requires-Dist: datasette-enrichments-jinja
 Requires-Dist: datasette-copyable
 Requires-Dist: datasette-export-database
 Requires-Dist: datasette-enrichments-gpt
+Requires-Dist: datasette-import
 
 # datasette-studio
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-studio.svg)](https://pypi.org/project/datasette-studio/)
 [![Changelog](https://img.shields.io/github/v/release/datasette/datasette-studio?include_prereleases&label=changelog)](https://github.com/datasette/datasette-studio/releases)
 [![Tests](https://github.com/datasette/datasette-studio/actions/workflows/test.yml/badge.svg)](https://github.com/datasette/datasette-studio/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-studio/blob/master/LICENSE)
 
 Datasette pre-configured with useful plugins.
 
 **Experimental alpha release**. This is an early experiment at the moment.
 
+[Try this out in GitHub Codespaces](https://github.com/codespaces/new?repo=datasette/studio)
+
 ## Installation
 
 This tool makes Datasette (currently the 1.0 alpha series) available as `datasette-studio` with a set of useful plugins pre-installed.
 
 It is _strongly_ recommended to install this using [pipx](https://pipx.pypa.io/), since doing so will ensure that this version of Datasette has its own isolated environment.
 
 ```bash
```

### Comparing `datasette-studio-0.1a2/README.md` & `datasette-studio-0.1a3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 [![Tests](https://github.com/datasette/datasette-studio/actions/workflows/test.yml/badge.svg)](https://github.com/datasette/datasette-studio/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-studio/blob/master/LICENSE)
 
 Datasette pre-configured with useful plugins.
 
 **Experimental alpha release**. This is an early experiment at the moment.
 
+[Try this out in GitHub Codespaces](https://github.com/codespaces/new?repo=datasette/studio)
+
 ## Installation
 
 This tool makes Datasette (currently the 1.0 alpha series) available as `datasette-studio` with a set of useful plugins pre-installed.
 
 It is _strongly_ recommended to install this using [pipx](https://pipx.pypa.io/), since doing so will ensure that this version of Datasette has its own isolated environment.
 
 ```bash
```

### Comparing `datasette-studio-0.1a2/datasette_studio.egg-info/PKG-INFO` & `datasette-studio-0.1a3/datasette_studio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-studio
-Version: 0.1a2
+Version: 0.1a3
 Summary: Datasette pre-configured with useful plugins
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-studio
 Project-URL: Changelog, https://github.com/datasette/datasette-studio/releases
 Project-URL: Issues, https://github.com/datasette/datasette-studio/issues
 Project-URL: CI, https://github.com/datasette/datasette-studio/actions
@@ -21,26 +21,29 @@
 Requires-Dist: datasette-enrichments
 Requires-Dist: datasette-enrichments-quickjs
 Requires-Dist: datasette-enrichments-re2
 Requires-Dist: datasette-enrichments-jinja
 Requires-Dist: datasette-copyable
 Requires-Dist: datasette-export-database
 Requires-Dist: datasette-enrichments-gpt
+Requires-Dist: datasette-import
 
 # datasette-studio
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-studio.svg)](https://pypi.org/project/datasette-studio/)
 [![Changelog](https://img.shields.io/github/v/release/datasette/datasette-studio?include_prereleases&label=changelog)](https://github.com/datasette/datasette-studio/releases)
 [![Tests](https://github.com/datasette/datasette-studio/actions/workflows/test.yml/badge.svg)](https://github.com/datasette/datasette-studio/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-studio/blob/master/LICENSE)
 
 Datasette pre-configured with useful plugins.
 
 **Experimental alpha release**. This is an early experiment at the moment.
 
+[Try this out in GitHub Codespaces](https://github.com/codespaces/new?repo=datasette/studio)
+
 ## Installation
 
 This tool makes Datasette (currently the 1.0 alpha series) available as `datasette-studio` with a set of useful plugins pre-installed.
 
 It is _strongly_ recommended to install this using [pipx](https://pipx.pypa.io/), since doing so will ensure that this version of Datasette has its own isolated environment.
 
 ```bash
```

### Comparing `datasette-studio-0.1a2/pyproject.toml` & `datasette-studio-0.1a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-studio"
-version = "0.1a2"
+version = "0.1a3"
 description = "Datasette pre-configured with useful plugins"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
@@ -19,14 +19,15 @@
     "datasette-enrichments",
     "datasette-enrichments-quickjs",
     "datasette-enrichments-re2",
     "datasette-enrichments-jinja",
     "datasette-copyable",
     "datasette-export-database",
     "datasette-enrichments-gpt",
+    "datasette-import",
 ]
 
 [project.urls]
 Homepage = "https://github.com/datasette/datasette-studio"
 Changelog = "https://github.com/datasette/datasette-studio/releases"
 Issues = "https://github.com/datasette/datasette-studio/issues"
 CI = "https://github.com/datasette/datasette-studio/actions"
```

