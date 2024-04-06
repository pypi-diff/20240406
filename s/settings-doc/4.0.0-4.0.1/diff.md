# Comparing `tmp/settings_doc-4.0.0.tar.gz` & `tmp/settings_doc-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "settings_doc-4.0.0.tar", max compression
+gzip compressed data, was "settings_doc-4.0.1.tar", max compression
```

## Comparing `settings_doc-4.0.0.tar` & `settings_doc-4.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2024-01-31 20:59:29.320679 settings_doc-4.0.0/LICENSE
--rw-r--r--   0        0        0    11647 2024-01-31 20:59:29.320679 settings_doc-4.0.0/README.md
--rw-r--r--   0        0        0     3984 2024-01-31 20:59:29.324679 settings_doc-4.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-31 20:59:29.324679 settings_doc-4.0.0/src/settings_doc/__init__.py
--rw-r--r--   0        0        0     2907 2024-01-31 20:59:29.324679 settings_doc-4.0.0/src/settings_doc/importing.py
--rw-r--r--   0        0        0     8180 2024-01-31 20:59:29.324679 settings_doc-4.0.0/src/settings_doc/main.py
--rw-r--r--   0        0        0      737 2024-01-31 20:59:29.324679 settings_doc-4.0.0/src/settings_doc/templates/debug.jinja
--rw-r--r--   0        0        0     1846 2024-01-31 20:59:29.324679 settings_doc-4.0.0/src/settings_doc/templates/dotenv.jinja
--rw-r--r--   0        0        0     3448 2024-01-31 20:59:29.324679 settings_doc-4.0.0/src/settings_doc/templates/markdown.jinja
--rw-r--r--   0        0        0    13288 1970-01-01 00:00:00.000000 settings_doc-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-06 09:59:42.071183 settings_doc-4.0.1/LICENSE
+-rw-r--r--   0        0        0    11601 2024-04-06 09:59:42.071183 settings_doc-4.0.1/README.md
+-rw-r--r--   0        0        0     4052 2024-04-06 09:59:42.071183 settings_doc-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-06 09:59:42.071183 settings_doc-4.0.1/src/settings_doc/__init__.py
+-rw-r--r--   0        0        0     2943 2024-04-06 09:59:42.071183 settings_doc-4.0.1/src/settings_doc/importing.py
+-rw-r--r--   0        0        0     8182 2024-04-06 09:59:42.071183 settings_doc-4.0.1/src/settings_doc/main.py
+-rw-r--r--   0        0        0      737 2024-04-06 09:59:42.071183 settings_doc-4.0.1/src/settings_doc/templates/debug.jinja
+-rw-r--r--   0        0        0     1846 2024-04-06 09:59:42.071183 settings_doc-4.0.1/src/settings_doc/templates/dotenv.jinja
+-rw-r--r--   0        0        0     3448 2024-04-06 09:59:42.071183 settings_doc-4.0.1/src/settings_doc/templates/markdown.jinja
+-rw-r--r--   0        0        0    13242 1970-01-01 00:00:00.000000 settings_doc-4.0.1/PKG-INFO
```

### Comparing `settings_doc-4.0.0/LICENSE` & `settings_doc-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `settings_doc-4.0.0/README.md` & `settings_doc-4.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-<h1 align="center" style="border-bottom: none;">⚙&nbsp;📝&nbsp;&nbsp;Settings&nbsp;DocGen&nbsp;&nbsp;📝&nbsp;⚙</h1>
-<h3 align="center">A command line tool for generating Markdown documentation and .env files from <a href="https://pydantic-docs.helpmanual.io/usage/settings">pydantic.BaseSettings</a>.</h3>
+<h1 align="center" style="border-bottom: none;">⚙&nbsp;📝&nbsp;&nbsp;Settings&nbsp;Doc&nbsp;&nbsp;📝&nbsp;⚙</h1>
+<h3 align="center">A command line tool for generating Markdown documentation and .env files from <a href="">pydantic_settings.BaseSettings</a>.</h3>
 
 <p align="center">
     <a href="https://app.circleci.com/pipelines/github/radeklat/settings-doc?branch=main">
         <img alt="CircleCI" src="https://img.shields.io/circleci/build/github/radeklat/settings-doc">
     </a>
     <a href="https://app.codecov.io/gh/radeklat/settings-doc/">
         <img alt="Codecov" src="https://img.shields.io/codecov/c/github/radeklat/settings-doc">
@@ -25,15 +25,15 @@
         <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/settings-doc">
     </a>
     <a href="https://pydantic.dev">
         <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json" alt="Pydantic Version 2" style="max-width:100%;">
     </a>
 </p>
 
-The same way you are able to generate OpenAPI documentation from [`pydantic.BaseModel`](https://pydantic-docs.helpmanual.io/usage/models/), `settings-doc` allows you to generate documentation from [`pydantic_settings.BaseSettings`](https://docs.pydantic.dev/latest/usage/pydantic_settings/).
+The same way you are able to generate OpenAPI documentation from [`pydantic.BaseModel`](https://pydantic-docs.helpmanual.io/usage/models/), `settings-doc` allows you to generate documentation from [`pydantic_settings.BaseSettings`](https://docs.pydantic.dev/latest/api/pydantic_settings/).
 
 It is powered by the [Jinja2](https://jinja.palletsprojects.com/en/latest/) templating engine and [Typer](https://typer.tiangolo.com/) framework. If you don't like the built-in templates, you can easily modify them or write completely custom ones. All attributes of the [`BaseSettings`](https://docs.pydantic.dev/latest/usage/pydantic_settings/) models are exposed to the templates.
 
 <!--
     How to generate TOC from PyCharm:
     https://github.com/vsch/idea-multimarkdown/wiki/Table-of-Contents-Extension
 -->
```

### Comparing `settings_doc-4.0.0/pyproject.toml` & `settings_doc-4.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "settings-doc"
-version = "4.0.0"
+version = "4.0.1"
 description = "A command line tool for generating Markdown documentation and .env files from pydantic BaseSettings."
 authors = ["Radek Lát <radek.lat@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 # https://pypi.org/classifiers/
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -48,14 +48,18 @@
 delfino-core = {extras = ["verify", "dependencies-update"], version = "^7.0"}  # https://github.com/radeklat/delfino-core/blob/main/CHANGELOG.md
 pytest-mock = "^3.6.1"
 
 [tool.poetry.group.dev.dependencies]
 pyupgrade = "^3.15.0"
 ruff = "^0.1.3"
 
+
+[tool.poetry.group.changelog.dependencies]
+python-kacl = "^0.4.6"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 # Setting compatible with black. See https://black.readthedocs.io/en/stable/compatible_configs.html
 multi_line_output = 3
```

### Comparing `settings_doc-4.0.0/src/settings_doc/importing.py` & `settings_doc-4.0.1/src/settings_doc/importing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import importlib
 from functools import lru_cache
 from inspect import isclass
-from typing import List, Set, Tuple, Type
+from typing import Dict, List, Tuple, Type
 
 from click import BadParameter, secho
 from pydantic_settings import BaseSettings
 from typer import colors
 
 _MODULE_ERROR_MSG = "No `pydantic.BaseSettings` subclasses found in module '{module_path}'."
 _RELATIVE_IMPORT_ERROR_MSG = "Relative imports are not supported."
 
 
 @lru_cache
-def import_module_path(module_paths: Tuple[str, ...]) -> Set[Type[BaseSettings]]:
+def import_module_path(module_paths: Tuple[str, ...]) -> Dict[Type[BaseSettings], None]:
     if not module_paths:
-        return set()
+        return {}
 
-    settings: Set[Type[BaseSettings]] = set()
+    settings: Dict[Type[BaseSettings], None] = {}
 
     for module_path in module_paths:
         try:
             module = importlib.import_module(module_path)
         except (ModuleNotFoundError, TypeError) as exc:
             cause = str(exc)
             if isinstance(exc, TypeError) and "relative import" in cause:
                 cause = _RELATIVE_IMPORT_ERROR_MSG
             raise BadParameter(f"Cannot read the module: {cause}") from exc
 
-        new_classes: Set[Type[BaseSettings]] = {
-            obj
+        new_classes: Dict[Type[BaseSettings], None] = {
+            obj: None
             for obj in vars(module).values()
             if isclass(obj) and issubclass(obj, BaseSettings) and obj.__module__.startswith(module_path)
         }
 
         if not new_classes:
             if len(module_paths) > 1:
                 secho(_MODULE_ERROR_MSG.format(module_path=module_path), fg=colors.YELLOW, err=True)
@@ -46,16 +46,16 @@
             else "No `pydantic.BaseSettings` subclasses found in any of the modules."
         )
 
     return settings
 
 
 @lru_cache
-def import_class_path(class_paths: Tuple[str, ...]) -> Set[Type[BaseSettings]]:
-    settings: Set[Type[BaseSettings]] = set()
+def import_class_path(class_paths: Tuple[str, ...]) -> Dict[Type[BaseSettings], None]:
+    settings: Dict[Type[BaseSettings], None] = {}
 
     for class_path in class_paths:
         module, class_name = class_path.rsplit(".", maxsplit=1)
         try:
             new_class = getattr(importlib.import_module(module), class_name)
         except (AttributeError, ModuleNotFoundError, TypeError) as exc:
             cause = str(exc)
@@ -65,15 +65,15 @@
 
         if not isclass(new_class):
             raise BadParameter(f"Target '{class_name}' in module '{module}' is not a class.")
 
         if not issubclass(new_class, BaseSettings):
             raise BadParameter(f"Target class must be a subclass of BaseSettings but '{new_class.__name__}' found.")
 
-        settings.add(new_class)
+        settings[new_class] = None
 
     return settings
 
 
 def module_path_callback(value: List[str]) -> List[str]:
     import_module_path(tuple(value))
     return value
```

### Comparing `settings_doc-4.0.0/src/settings_doc/main.py` & `settings_doc-4.0.1/src/settings_doc/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import shutil
 import sys
 from collections.abc import Iterable as IterableCollection
 from enum import Enum, auto
 from os import listdir
 from pathlib import Path
-from typing import Any, Dict, Final, Iterator, List, Literal, Optional, Set, Tuple, Type
+from typing import Any, Dict, Final, Iterator, List, Literal, Optional, Tuple, Type
 
 from click import Abort, secho
 from jinja2 import Environment, FileSystemLoader, Template, select_autoescape
 from pydantic.fields import FieldInfo
 from pydantic_core import PydanticUndefined
 from pydantic_settings import BaseSettings
 from typer import Option, Typer, colors
@@ -141,17 +141,16 @@
         resolve_path=True,
         help="Folder to use when looking up templates for generating output. Can be used "
         "more than once, in a priority order. Built-in templates will be used last if no "
         "matches found.",
     ),
 ):
     """Formats `pydantic.BaseSettings` into various formats. By default, the output is to STDOUT."""
-    settings: Set[Type[BaseSettings]] = importing.import_class_path(tuple(class_path)).union(
-        importing.import_module_path(tuple(module_path))
-    )
+    settings: Dict[Type[BaseSettings], None] = importing.import_class_path(tuple(class_path))
+    settings.update(importing.import_module_path(tuple(module_path)))
 
     if not settings:
         secho("No sources of data were specified. Use the '--module' or '--class' options.", fg=colors.RED, err=True)
         raise Abort()
 
     fields = itertools.chain.from_iterable(_model_fields(cls) for cls in settings)
     classes: Dict[Type[BaseSettings], List[FieldInfo]] = {cls: list(cls.model_fields.values()) for cls in settings}
```

### Comparing `settings_doc-4.0.0/src/settings_doc/templates/debug.jinja` & `settings_doc-4.0.1/src/settings_doc/templates/debug.jinja`

 * *Files identical despite different names*

### Comparing `settings_doc-4.0.0/src/settings_doc/templates/dotenv.jinja` & `settings_doc-4.0.1/src/settings_doc/templates/dotenv.jinja`

 * *Files identical despite different names*

### Comparing `settings_doc-4.0.0/src/settings_doc/templates/markdown.jinja` & `settings_doc-4.0.1/src/settings_doc/templates/markdown.jinja`

 * *Files identical despite different names*

### Comparing `settings_doc-4.0.0/PKG-INFO` & `settings_doc-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settings-doc
-Version: 4.0.0
+Version: 4.0.1
 Summary: A command line tool for generating Markdown documentation and .env files from pydantic BaseSettings.
 Home-page: https://github.com/radeklat/settings-doc
 License: MIT
 Keywords: documentation,environment variables,generated,markdown,BaseSettings
 Author: Radek Lát
 Author-email: radek.lat@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -32,16 +32,16 @@
 Classifier: Typing :: Typed
 Requires-Dist: Jinja2 (>=3.0.2,<4.0.0)
 Requires-Dist: pydantic (>=2.3,<3.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: typer[all] (>=0.9,<0.10)
 Description-Content-Type: text/markdown
 
-<h1 align="center" style="border-bottom: none;">⚙&nbsp;📝&nbsp;&nbsp;Settings&nbsp;DocGen&nbsp;&nbsp;📝&nbsp;⚙</h1>
-<h3 align="center">A command line tool for generating Markdown documentation and .env files from <a href="https://pydantic-docs.helpmanual.io/usage/settings">pydantic.BaseSettings</a>.</h3>
+<h1 align="center" style="border-bottom: none;">⚙&nbsp;📝&nbsp;&nbsp;Settings&nbsp;Doc&nbsp;&nbsp;📝&nbsp;⚙</h1>
+<h3 align="center">A command line tool for generating Markdown documentation and .env files from <a href="">pydantic_settings.BaseSettings</a>.</h3>
 
 <p align="center">
     <a href="https://app.circleci.com/pipelines/github/radeklat/settings-doc?branch=main">
         <img alt="CircleCI" src="https://img.shields.io/circleci/build/github/radeklat/settings-doc">
     </a>
     <a href="https://app.codecov.io/gh/radeklat/settings-doc/">
         <img alt="Codecov" src="https://img.shields.io/codecov/c/github/radeklat/settings-doc">
@@ -63,15 +63,15 @@
         <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/settings-doc">
     </a>
     <a href="https://pydantic.dev">
         <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json" alt="Pydantic Version 2" style="max-width:100%;">
     </a>
 </p>
 
-The same way you are able to generate OpenAPI documentation from [`pydantic.BaseModel`](https://pydantic-docs.helpmanual.io/usage/models/), `settings-doc` allows you to generate documentation from [`pydantic_settings.BaseSettings`](https://docs.pydantic.dev/latest/usage/pydantic_settings/).
+The same way you are able to generate OpenAPI documentation from [`pydantic.BaseModel`](https://pydantic-docs.helpmanual.io/usage/models/), `settings-doc` allows you to generate documentation from [`pydantic_settings.BaseSettings`](https://docs.pydantic.dev/latest/api/pydantic_settings/).
 
 It is powered by the [Jinja2](https://jinja.palletsprojects.com/en/latest/) templating engine and [Typer](https://typer.tiangolo.com/) framework. If you don't like the built-in templates, you can easily modify them or write completely custom ones. All attributes of the [`BaseSettings`](https://docs.pydantic.dev/latest/usage/pydantic_settings/) models are exposed to the templates.
 
 <!--
     How to generate TOC from PyCharm:
     https://github.com/vsch/idea-multimarkdown/wiki/Table-of-Contents-Extension
 -->
```

