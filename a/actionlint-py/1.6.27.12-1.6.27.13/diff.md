# Comparing `tmp/actionlint_py-1.6.27.12.tar.gz` & `tmp/actionlint_py-1.6.27.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionlint_py-1.6.27.12.tar", last modified: Thu Mar 21 08:59:37 2024, max compression
+gzip compressed data, was "actionlint_py-1.6.27.13.tar", last modified: Sat Apr  6 06:49:50 2024, max compression
```

## Comparing `actionlint_py-1.6.27.12.tar` & `actionlint_py-1.6.27.13.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:59:37.904570 actionlint_py-1.6.27.12/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-03-21 08:59:37.904570 actionlint_py-1.6.27.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:59:37.900570 actionlint_py-1.6.27.12/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/VERSION_ACTIONLINT.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/VERSION_BUILD_SYSTEM.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/VERSION_DEV.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/auto_update_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/checksums.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:59:37.900570 actionlint_py-1.6.27.12/_custom_build/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/commands/bdist_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/commands/fetch_binaries.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/commands/install_actionlint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:59:37.900570 actionlint_py-1.6.27.12/_custom_build/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/utils/file_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/_custom_build/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:59:37.904570 actionlint_py-1.6.27.12/actionlint_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-03-21 08:59:37.000000 actionlint_py-1.6.27.12/actionlint_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-21 08:59:37.000000 actionlint_py-1.6.27.12/actionlint_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 08:59:37.000000 actionlint_py-1.6.27.12/actionlint_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-21 08:59:37.000000 actionlint_py-1.6.27.12/actionlint_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-21 08:59:37.000000 actionlint_py-1.6.27.12/actionlint_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-21 08:59:24.000000 actionlint_py-1.6.27.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 08:59:37.904570 actionlint_py-1.6.27.12/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:50.809586 actionlint_py-1.6.27.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-06 06:49:50.809586 actionlint_py-1.6.27.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:50.805586 actionlint_py-1.6.27.13/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/VERSION_ACTIONLINT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/VERSION_BUILD_SYSTEM.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/VERSION_DEV.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/auto_update_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/checksums.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:50.805586 actionlint_py-1.6.27.13/_custom_build/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/bdist_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/fetch_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/install_actionlint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:50.805586 actionlint_py-1.6.27.13/_custom_build/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/utils/file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:50.809586 actionlint_py-1.6.27.13/actionlint_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-06 06:49:50.000000 actionlint_py-1.6.27.13/actionlint_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-06 06:49:50.000000 actionlint_py-1.6.27.13/actionlint_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:49:50.000000 actionlint_py-1.6.27.13/actionlint_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-06 06:49:50.000000 actionlint_py-1.6.27.13/actionlint_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 06:49:50.000000 actionlint_py-1.6.27.13/actionlint_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 06:49:50.809586 actionlint_py-1.6.27.13/setup.cfg
```

### Comparing `actionlint_py-1.6.27.12/LICENSE` & `actionlint_py-1.6.27.13/LICENSE`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.12/PKG-INFO` & `actionlint_py-1.6.27.13/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionlint_py
-Version: 1.6.27.12
+Version: 1.6.27.13
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Author-email: Ryan Rhee <pypi@rhee.io>, Mateusz Grzeliński <grzelinskimat@gmail.com>
 Maintainer-email: Mateusz Grzeliński <grzelinskimat@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Ryan Rhee
         
@@ -39,14 +39,15 @@
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Provides-Extra: auto-update
 Requires-Dist: requests; extra == "auto-update"
 Requires-Dist: semver; extra == "auto-update"
 Requires-Dist: requests_html; extra == "auto-update"
+Requires-Dist: lxml[html_clean]; extra == "auto-update"
 
 > Note: for `pre-commit` hooks I recommend officially supported hooks:
 > See docs: https://github.com/rhysd/actionlint/blob/main/docs/usage.md#pre-commit
 
 # actionlint-py
 
 A python wrapper to provide a pip-installable [actionlint] binary.
@@ -74,15 +75,15 @@
 
 Use this repo if you can not use officially supported hooks (docker, golang, system) and you are fine with python `pip` wrapper.
 
 Sample `.pre-commit-config.yaml` using `pip` as package manager:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.27.12
+  rev: v1.6.27.13
   hooks:
     - id: actionlint
       additional_dependencies: [ pyflakes>=3.0.1, shellcheck-py>=0.9.0.5 ]
       # actionlint has built in support for pyflakes and shellcheck, sadly they will not be auto updated. Check https://pypi.org/project/actionlint-py/ for latest version. Alternatively:
       # args: [-shellcheck=/path/shellcheck -pyflakes=/path/pyflakes]
       # note - invalid path in arguments will fail silently
 ```
@@ -94,17 +95,17 @@
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.6.27.12]
+      #additional_dependencies: [actionlint-py==1.6.27.13]
       # safer, but pre-commit autoupdate will not work
-      # note: the pip versioning scheme is different from actionlint binary: not "v1.6.27" but "1.6.27.12" (last number is build system version)
+      # note: the pip versioning scheme is different from actionlint binary: not "v1.6.27" but "1.6.27.13" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
```

### Comparing `actionlint_py-1.6.27.12/README.md` & `actionlint_py-1.6.27.13/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 Use this repo if you can not use officially supported hooks (docker, golang, system) and you are fine with python `pip` wrapper.
 
 Sample `.pre-commit-config.yaml` using `pip` as package manager:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.27.12
+  rev: v1.6.27.13
   hooks:
     - id: actionlint
       additional_dependencies: [ pyflakes>=3.0.1, shellcheck-py>=0.9.0.5 ]
       # actionlint has built in support for pyflakes and shellcheck, sadly they will not be auto updated. Check https://pypi.org/project/actionlint-py/ for latest version. Alternatively:
       # args: [-shellcheck=/path/shellcheck -pyflakes=/path/pyflakes]
       # note - invalid path in arguments will fail silently
 ```
@@ -48,17 +48,17 @@
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.6.27.12]
+      #additional_dependencies: [actionlint-py==1.6.27.13]
       # safer, but pre-commit autoupdate will not work
-      # note: the pip versioning scheme is different from actionlint binary: not "v1.6.27" but "1.6.27.12" (last number is build system version)
+      # note: the pip versioning scheme is different from actionlint binary: not "v1.6.27" but "1.6.27.13" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
```

### Comparing `actionlint_py-1.6.27.12/_custom_build/auto_update_main.py` & `actionlint_py-1.6.27.13/_custom_build/auto_update_main.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.12/_custom_build/checksums.cfg` & `actionlint_py-1.6.27.13/_custom_build/checksums.cfg`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.12/_custom_build/commands/fetch_binaries.py` & `actionlint_py-1.6.27.13/_custom_build/commands/fetch_binaries.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.12/_custom_build/commands/install_actionlint.py` & `actionlint_py-1.6.27.13/_custom_build/commands/install_actionlint.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.12/_custom_build/utils/file_ops.py` & `actionlint_py-1.6.27.13/_custom_build/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.12/_custom_build/version.py` & `actionlint_py-1.6.27.13/_custom_build/version.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.12/actionlint_py.egg-info/PKG-INFO` & `actionlint_py-1.6.27.13/actionlint_py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionlint_py
-Version: 1.6.27.12
+Version: 1.6.27.13
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Author-email: Ryan Rhee <pypi@rhee.io>, Mateusz Grzeliński <grzelinskimat@gmail.com>
 Maintainer-email: Mateusz Grzeliński <grzelinskimat@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Ryan Rhee
         
@@ -39,14 +39,15 @@
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Provides-Extra: auto-update
 Requires-Dist: requests; extra == "auto-update"
 Requires-Dist: semver; extra == "auto-update"
 Requires-Dist: requests_html; extra == "auto-update"
+Requires-Dist: lxml[html_clean]; extra == "auto-update"
 
 > Note: for `pre-commit` hooks I recommend officially supported hooks:
 > See docs: https://github.com/rhysd/actionlint/blob/main/docs/usage.md#pre-commit
 
 # actionlint-py
 
 A python wrapper to provide a pip-installable [actionlint] binary.
@@ -74,15 +75,15 @@
 
 Use this repo if you can not use officially supported hooks (docker, golang, system) and you are fine with python `pip` wrapper.
 
 Sample `.pre-commit-config.yaml` using `pip` as package manager:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.27.12
+  rev: v1.6.27.13
   hooks:
     - id: actionlint
       additional_dependencies: [ pyflakes>=3.0.1, shellcheck-py>=0.9.0.5 ]
       # actionlint has built in support for pyflakes and shellcheck, sadly they will not be auto updated. Check https://pypi.org/project/actionlint-py/ for latest version. Alternatively:
       # args: [-shellcheck=/path/shellcheck -pyflakes=/path/pyflakes]
       # note - invalid path in arguments will fail silently
 ```
@@ -94,17 +95,17 @@
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.6.27.12]
+      #additional_dependencies: [actionlint-py==1.6.27.13]
       # safer, but pre-commit autoupdate will not work
-      # note: the pip versioning scheme is different from actionlint binary: not "v1.6.27" but "1.6.27.12" (last number is build system version)
+      # note: the pip versioning scheme is different from actionlint binary: not "v1.6.27" but "1.6.27.13" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
```

### Comparing `actionlint_py-1.6.27.12/actionlint_py.egg-info/SOURCES.txt` & `actionlint_py-1.6.27.13/actionlint_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.12/pyproject.toml` & `actionlint_py-1.6.27.13/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: Implementation :: PyPy",
     "Intended Audience :: Developers",
 ]
 dependencies = []
 
 [project.optional-dependencies]
 dev = ["black"]
-auto_update = ["requests", "semver", "requests_html"]
+auto_update = ["requests", "semver", "requests_html", "lxml[html_clean]"]
 
 [project.urls]
 "Homepage" = "https://github.com/Mateusz-Grzelinski/actionlint-py"
 "Bug Reports" = "https://github.com/Mateusz-Grzelinski/actionlint-py/issues"
 
 [tool.black]
 line-length = 120
```

