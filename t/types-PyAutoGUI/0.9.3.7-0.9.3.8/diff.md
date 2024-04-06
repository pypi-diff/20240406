# Comparing `tmp/types-PyAutoGUI-0.9.3.7.tar.gz` & `tmp/types-PyAutoGUI-0.9.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-PyAutoGUI-0.9.3.7.tar", last modified: Thu Jul 20 15:21:49 2023, max compression
+gzip compressed data, was "types-PyAutoGUI-0.9.3.8.tar", last modified: Tue Dec 19 02:21:02 2023, max compression
```

## Comparing `types-PyAutoGUI-0.9.3.7.tar` & `types-PyAutoGUI-0.9.3.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:49.201236 types-PyAutoGUI-0.9.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-20 15:21:48.000000 types-PyAutoGUI-0.9.3.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:48.000000 types-PyAutoGUI-0.9.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-20 15:21:49.201236 types-PyAutoGUI-0.9.3.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:49.201236 types-PyAutoGUI-0.9.3.7/pyautogui-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 15:21:48.000000 types-PyAutoGUI-0.9.3.7/pyautogui-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-07-20 15:15:13.000000 types-PyAutoGUI-0.9.3.7/pyautogui-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:49.201236 types-PyAutoGUI-0.9.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-20 15:21:48.000000 types-PyAutoGUI-0.9.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:49.201236 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-20 15:21:49.000000 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-20 15:21:49.000000 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:49.000000 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 15:21:49.000000 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 15:21:49.000000 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:21:02.089644 types-PyAutoGUI-0.9.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-12-19 02:21:01.000000 types-PyAutoGUI-0.9.3.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-19 02:21:01.000000 types-PyAutoGUI-0.9.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2023-12-19 02:21:02.089644 types-PyAutoGUI-0.9.3.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:21:02.085644 types-PyAutoGUI-0.9.3.8/pyautogui-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-19 02:21:01.000000 types-PyAutoGUI-0.9.3.8/pyautogui-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2023-12-19 02:20:33.000000 types-PyAutoGUI-0.9.3.8/pyautogui-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:21:02.089644 types-PyAutoGUI-0.9.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-12-19 02:21:01.000000 types-PyAutoGUI-0.9.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:21:02.089644 types-PyAutoGUI-0.9.3.8/types_PyAutoGUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2023-12-19 02:21:02.000000 types-PyAutoGUI-0.9.3.8/types_PyAutoGUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-19 02:21:02.000000 types-PyAutoGUI-0.9.3.8/types_PyAutoGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 02:21:02.000000 types-PyAutoGUI-0.9.3.8/types_PyAutoGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-19 02:21:02.000000 types-PyAutoGUI-0.9.3.8/types_PyAutoGUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-19 02:21:02.000000 types-PyAutoGUI-0.9.3.8/types_PyAutoGUI.egg-info/top_level.txt
```

### Comparing `types-PyAutoGUI-0.9.3.7/CHANGELOG.md` & `types-PyAutoGUI-0.9.3.8/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.9.3.8 (2023-12-19)
+
+Review `SupportsInt` and `SupportsFloat` usages in 3rd-party stubs (#11003)
+
 ## 0.9.3.7 (2023-07-20)
 
 Add an upstream_repository field to METADATA.toml (#10487)
 
 Closes: #10478
 
 ## 0.9.3.6 (2023-05-25)
```

### Comparing `types-PyAutoGUI-0.9.3.7/PKG-INFO` & `types-PyAutoGUI-0.9.3.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: types-PyAutoGUI
-Version: 0.9.3.7
+Version: 0.9.3.8
 Summary: Typing stubs for PyAutoGUI
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyAutoGUI.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Typing stubs for PyAutoGUI
 
-This is a PEP 561 type stub package for the `PyAutoGUI` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`PyAutoGUI`](https://github.com/asweigart/pyautogui) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`PyAutoGUI`. The source for this package can be found at
+`PyAutoGUI`.
+
+This version of `types-PyAutoGUI` aims to provide accurate annotations
+for `PyAutoGUI==0.9.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyAutoGUI. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `7bdf6ba85ceeebfaf68f632fe0a02f08ce457694` and was tested
+with mypy 1.7.1, pyright 1.1.339, and
+pytype 2023.12.8.
```

### Comparing `types-PyAutoGUI-0.9.3.7/pyautogui-stubs/__init__.pyi` & `types-PyAutoGUI-0.9.3.8/pyautogui-stubs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+from _typeshed import ConvertibleToInt
 from collections.abc import Callable, Iterable, Sequence
 from datetime import datetime
 from typing import NamedTuple, SupportsInt, TypeVar
 from typing_extensions import Final, ParamSpec, SupportsIndex, TypeAlias
 
 from pyscreeze import (
     center as center,
@@ -15,15 +16,18 @@
     pixel as pixel,
     pixelMatchesColor as pixelMatchesColor,
     screenshot as screenshot,
 )
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
-_NormalizeableXArg: TypeAlias = str | SupportsInt | Sequence[SupportsInt]
+# Explicitly mentioning str despite being in the ConvertibleToInt Alias because it has a different meaning (filename on screen)
+# Specifying non-None Y arg when X is a string or sequence raises an error
+# TODO: This could be better represented through overloads
+_NormalizeableXArg: TypeAlias = str | ConvertibleToInt | Sequence[ConvertibleToInt]
 
 # Constants
 KEY_NAMES: list[str]
 KEYBOARD_KEYS: list[str]
 LEFT: Final = "left"
 MIDDLE: Final = "middle"
 RIGHT: Final = "right"
```

### Comparing `types-PyAutoGUI-0.9.3.7/setup.py` & `types-PyAutoGUI-0.9.3.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 from setuptools import setup
 
 name = "types-PyAutoGUI"
 description = "Typing stubs for PyAutoGUI"
 long_description = '''
 ## Typing stubs for PyAutoGUI
 
-This is a PEP 561 type stub package for the `PyAutoGUI` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`PyAutoGUI`](https://github.com/asweigart/pyautogui) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`PyAutoGUI`. The source for this package can be found at
+`PyAutoGUI`.
+
+This version of `types-PyAutoGUI` aims to provide accurate annotations
+for `PyAutoGUI==0.9.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyAutoGUI. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `7bdf6ba85ceeebfaf68f632fe0a02f08ce457694` and was tested
+with mypy 1.7.1, pyright 1.1.339, and
+pytype 2023.12.8.
 '''.lstrip()
 
 setup(name=name,
-      version="0.9.3.7",
+      version="0.9.3.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyAutoGUI.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-Pillow', 'types-PyScreeze'],
       packages=['pyautogui-stubs'],
       package_data={'pyautogui-stubs': ['__init__.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
+      python_requires=">=3.7",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/PKG-INFO` & `types-PyAutoGUI-0.9.3.8/types_PyAutoGUI.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: types-PyAutoGUI
-Version: 0.9.3.7
+Version: 0.9.3.8
 Summary: Typing stubs for PyAutoGUI
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyAutoGUI.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Typing stubs for PyAutoGUI
 
-This is a PEP 561 type stub package for the `PyAutoGUI` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`PyAutoGUI`](https://github.com/asweigart/pyautogui) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`PyAutoGUI`. The source for this package can be found at
+`PyAutoGUI`.
+
+This version of `types-PyAutoGUI` aims to provide accurate annotations
+for `PyAutoGUI==0.9.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyAutoGUI. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `7bdf6ba85ceeebfaf68f632fe0a02f08ce457694` and was tested
+with mypy 1.7.1, pyright 1.1.339, and
+pytype 2023.12.8.
```

