# Comparing `tmp/clementine-2023.8.24.tar.gz` & `tmp/clementine-2024.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clementine-2023.8.24.tar", last modified: Thu Aug 24 19:54:02 2023, max compression
+gzip compressed data, was "clementine-2024.4.6.tar", last modified: Sat Apr  6 15:03:07 2024, max compression
```

## Comparing `clementine-2023.8.24.tar` & `clementine-2024.4.6.tar`

### file list

```diff
@@ -1,36 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 19:54:02.178273 clementine-2023.8.24/
--rw-r--r--   0 runner    (1001) docker     (999)     1068 2023-08-24 19:53:50.000000 clementine-2023.8.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     3706 2023-08-24 19:54:02.174272 clementine-2023.8.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1498 2023-08-24 19:53:50.000000 clementine-2023.8.24/README.md
--rw-r--r--   0 runner    (1001) docker     (999)     2301 2023-08-24 19:53:50.000000 clementine-2023.8.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-24 19:54:02.178273 clementine-2023.8.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-24 19:53:50.000000 clementine-2023.8.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 19:54:02.170272 clementine-2023.8.24/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 19:54:02.174272 clementine-2023.8.24/src/clementine/
--rw-r--r--   0 runner    (1001) docker     (999)      106 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      119 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 19:54:02.174272 clementine-2023.8.24/src/clementine/about/
--rw-r--r--   0 runner    (1001) docker     (999)      628 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/about/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4246 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/about/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 19:54:02.174272 clementine-2023.8.24/src/clementine/cli/
--rw-r--r--   0 runner    (1001) docker     (999)      585 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 19:54:02.174272 clementine-2023.8.24/src/clementine/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (999)      176 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      641 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/cli/commands/_info.py
--rw-r--r--   0 runner    (1001) docker     (999)     1245 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/cli/commands/_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (999)     1326 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/env.py
--rw-r--r--   0 runner    (1001) docker     (999)      322 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/errors.py
--rw-r--r--   0 runner    (1001) docker     (999)     1566 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/importing.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/py.typed
--rw-r--r--   0 runner    (1001) docker     (999)     4119 2023-08-24 19:53:50.000000 clementine-2023.8.24/src/clementine/screenshot.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 19:54:02.174272 clementine-2023.8.24/src/clementine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3706 2023-08-24 19:54:02.000000 clementine-2023.8.24/src/clementine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      741 2023-08-24 19:54:02.000000 clementine-2023.8.24/src/clementine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-24 19:54:02.000000 clementine-2023.8.24/src/clementine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       51 2023-08-24 19:54:02.000000 clementine-2023.8.24/src/clementine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      579 2023-08-24 19:54:02.000000 clementine-2023.8.24/src/clementine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-24 19:54:02.000000 clementine-2023.8.24/src/clementine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 19:54:02.174272 clementine-2023.8.24/tests/
--rw-r--r--   0 runner    (1001) docker     (999)     1129 2023-08-24 19:53:50.000000 clementine-2023.8.24/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (999)      579 2023-08-24 19:53:50.000000 clementine-2023.8.24/tests/test_importing.py
--rw-r--r--   0 runner    (1001) docker     (999)     1370 2023-08-24 19:53:50.000000 clementine-2023.8.24/tests/test_screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:03:07.796203 clementine-2024.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-06 15:03:01.000000 clementine-2024.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-06 15:03:07.796203 clementine-2024.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-06 15:03:01.000000 clementine-2024.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-06 15:03:01.000000 clementine-2024.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:03:07.796203 clementine-2024.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:03:01.000000 clementine-2024.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:03:07.784203 clementine-2024.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:03:07.788203 clementine-2024.4.6/src/clementine/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:03:07.788203 clementine-2024.4.6/src/clementine/about/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/about/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/about/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:03:07.788203 clementine-2024.4.6/src/clementine/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:03:07.788203 clementine-2024.4.6/src/clementine/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/cli/commands/_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/cli/commands/_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/importing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-06 15:03:01.000000 clementine-2024.4.6/src/clementine/screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:03:07.788203 clementine-2024.4.6/src/clementine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-06 15:03:07.000000 clementine-2024.4.6/src/clementine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-06 15:03:07.000000 clementine-2024.4.6/src/clementine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:03:07.000000 clementine-2024.4.6/src/clementine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 15:03:07.000000 clementine-2024.4.6/src/clementine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-06 15:03:07.000000 clementine-2024.4.6/src/clementine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 15:03:07.000000 clementine-2024.4.6/src/clementine.egg-info/top_level.txt
```

### Comparing `clementine-2023.8.24/LICENSE` & `clementine-2024.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clementine-2023.8.24/README.md` & `clementine-2024.4.6/README.md`

 * *Files identical despite different names*

### Comparing `clementine-2023.8.24/pyproject.toml` & `clementine-2024.4.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 [project]
 name = "clementine"
 dynamic = ["version"]
 description = "🍊 A sweet little Python package"
 authors = [{name = "Suzen Fylke", email = "codesue@users.noreply.github.com"}]
 readme = "README.md"
-license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries",
@@ -27,19 +26,22 @@
 blossom = [
     "bokeh",
     "gradio",
     "playwright",
 ]
 fruit = [
     "catppuccin-matplotlib",
+    "keras>=3",
     "numpy",
     "pandas",
     "scikit-learn",
+    "torch>=2",
 ]
 leaves = [
+    "mkdocs-click",
     "mkdocs-walt",
     "mkdocstrings[python]",
 ]
 pulp = [
     "datasets",
     "spacy",
     "transformers",
@@ -65,17 +67,20 @@
     "rich",
 ]
 tree = [
     "bokeh",
     "gradio",
     "playwright",
     "catppuccin-matplotlib",
+    "keras>=3",
     "numpy",
     "pandas",
     "scikit-learn",
+    "torch>=2",
+    "mkdocs-click",
     "mkdocs-walt",
     "mkdocstrings[python]",
     "datasets",
     "spacy",
     "transformers",
     "wandb",
     "build",
@@ -116,7 +121,14 @@
 exclude_dirs = ["scripts"]
 
 [tool.bandit.assert_used]
 skips = ["tests/**"]
 
 [tool.mypy]
 mypy_path = "stubs"
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+python_files = "*.py"
+markers = [
+  "slow: mark the test as slow. Deselect with '-m \"not slow\"'.",
+]
```

### Comparing `clementine-2023.8.24/src/clementine/about/__init__.py` & `clementine-2024.4.6/src/clementine/about/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Some metadata for the clementine package."""
 
 import webbrowser
 
 __title__ = "clementine"
 __description__ = "🍊 clementine is a sweet little Python package."
 __author__ = "Suzen Fylke"
-__version__ = "2023.8.24"  # Calver with format YYYY.MM.DD
+__version__ = "2024.4.6"  # Calver with format YYYY.MM.DD
 __pretty_version__ = f"{__title__} v{__version__}"
 __documentation__ = "https://codesue.github.io/clementine"
 __repository__ = "https://github.com/codesue/clementine"
 
 
 def docs():
     """Opens the documentation website in a browser."""
```

### Comparing `clementine-2023.8.24/src/clementine/about/dependencies.py` & `clementine-2024.4.6/src/clementine/about/dependencies.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Package dependencies for clementine."""
 
-from collections import namedtuple
 from dataclasses import dataclass
 from typing import Union
 
 __all__ = [
-    "ClementineExtras",
     "Extra",
     "dependencies",
     "extras",
     "optional_dependencies",
     "python_version",
     "recommended_dependencies",
 ]
@@ -20,14 +18,16 @@
     "bokeh": "bokeh",
     "build": "build",
     "catppuccin-matplotlib": "catppuccin-matplotlib",
     "click": "click",
     "datasets": "datasets",
     "gradio": "gradio",
     "isort": "isort",
+    "keras": "keras>=3",
+    "mkdocs-click": "mkdocs-click",
     "mkdocs-walt": "mkdocs-walt",
     "mkdocstrings": "mkdocstrings[python]",
     "mypy": "mypy",
     "numpy": "numpy",
     "notebook": "notebook",
     "pandas": "pandas",
     "pip-tools": "pip-tools",
@@ -36,14 +36,15 @@
     "pyperclip": "pyperclip",
     "pytest": "pytest",
     "rich": "rich",
     "ruff": "ruff",
     "scikit-learn": "scikit-learn",
     "spacy": "spacy",
     "tomlkit": "tomlkit",
+    "torch": "torch>=2",
     "transformers": "transformers",
     "twine": "twine",
     "wandb": "wandb",
 }
 
 
 @dataclass(frozen=True)
@@ -51,52 +52,30 @@
     """Basic information about an extra dependency."""
 
     name: str
     description: str
     deps: tuple[str, ...]
 
 
-ClementineExtras = namedtuple(
-    "ClementineExtras",
-    ["blossom", "fruit", "leaves", "pulp", "rind", "seeds", "sprout", "tree"],
-)
-
-
-def _make_deps_list(package_names: Union[list[str], tuple[str, ...]]) -> list[str]:
-    """Returns a list of dependencies with their constraints.
-
-    Raises: ValueError if a `package_name` is not in the list of known dependencies.
-    """
-    deps = []
-    for package_name in package_names:
-        if package_name not in _VERSIONS:
-            raise ValueError(
-                f"Package '{package_name}' is not in the list of known dependencies: "
-                f"{list(_VERSIONS.keys())}"
-            )
-        deps.append(_VERSIONS[package_name])
-    return deps
-
-
 _blossom = Extra(
     name="blossom",
     description="visualization and demonstration tools",
     deps=("bokeh", "gradio", "playwright"),
 )
 
 _fruit = Extra(
     name="fruit",
     description="machine learning libraries",
-    deps=("catppuccin-matplotlib", "numpy", "pandas", "scikit-learn"),
+    deps=("catppuccin-matplotlib", "keras", "numpy", "pandas", "scikit-learn", "torch"),
 )
 
 _leaves = Extra(
     name="leaves",
     description="documentation tools",
-    deps=("mkdocs-walt", "mkdocstrings"),
+    deps=("mkdocs-click", "mkdocs-walt", "mkdocstrings"),
 )
 
 _pulp = Extra(
     name="pulp",
     description="auxiliary ml libraries",
     deps=("datasets", "spacy", "transformers", "wandb"),
 )
@@ -138,44 +117,58 @@
         *_pulp.deps,
         *_rind.deps,
         *_seeds.deps,
         *_sprout.deps,
     ),
 )
 
-extras = ClementineExtras(
-    blossom=_blossom,
-    fruit=_fruit,
-    leaves=_leaves,
-    pulp=_pulp,
-    rind=_rind,
-    seeds=_seeds,
-    sprout=_sprout,
-    tree=_tree,
-)
 
+def _make_deps_list(package_names: Union[list[str], tuple[str, ...]]) -> list[str]:
+    """Returns a list of dependencies with their constraints.
 
-def dependencies():
+    Args:
+      package_names: The names of the packages to include.
+
+    Raises:
+      ValueError: If a `package_name` is not a known dependencies.
+    """
+    deps = []
+    for package_name in package_names:
+        if package_name not in _VERSIONS:
+            raise ValueError(
+                f"Package '{package_name}' is not a known dependencies: "
+                f"{list(_VERSIONS.keys())}"
+            )
+        deps.append(_VERSIONS[package_name])
+    return deps
+
+
+def dependencies() -> list[str]:
     """Returns a list of clementine's required dependencies."""
     return []
 
 
-def optional_dependencies():
+def optional_dependencies() -> dict[str, list]:
     """Returns a dictionary of clementine's optional dependencies."""
     return {
         "all": _make_deps_list(["click", "playwright", "pyperclip"]),
     }
 
 
-def recommended_dependencies():
+def extras() -> tuple[Extra, ...]:
+    """Returns a tuple of clementine's recommended dependencies as `Extra`s."""
+    return (_blossom, _fruit, _leaves, _pulp, _rind, _seeds, _sprout, _tree)
+
+
+def recommended_dependencies() -> dict[str, list]:
     """Returns a dictionary of recommended dependencies.
 
     The recommended dependencies are a collection of libraries and frameworks
     you might want to use when starting a new project. These dependencies aren't
     necessarily used in clementine, but they're made available as extra packages
     for easier installation."""
-    return {extra.name: _make_deps_list(extra.deps) for extra in extras}
+    return {extra.name: _make_deps_list(extra.deps) for extra in extras()}
 
 
-def python_version():
+def python_version() -> str:
     """Returns clementine's required Python version."""
     return ">=3.9"
```

### Comparing `clementine-2023.8.24/src/clementine/cli/__init__.py` & `clementine-2024.4.6/src/clementine/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `clementine-2023.8.24/src/clementine/cli/commands/_info.py` & `clementine-2024.4.6/src/clementine/cli/commands/_info.py`

 * *Files identical despite different names*

### Comparing `clementine-2023.8.24/src/clementine/cli/commands/_screenshot.py` & `clementine-2024.4.6/src/clementine/cli/commands/_screenshot.py`

 * *Files identical despite different names*

### Comparing `clementine-2023.8.24/src/clementine/importing.py` & `clementine-2024.4.6/src/clementine/importing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,70 @@
 """Importing utilities."""
 
 import importlib
 from types import ModuleType
 from typing import Optional, Union
 
-from clementine import errors
-
 __all__ = ["MissingModulePlaceholder", "maybe_import_module"]
 
 
 # Inspired by https://github.com/koaning/embetter/blob/main/embetter/error.py
 class MissingModulePlaceholder:
     """A placeholder for a module that is not installed. This allows us to
     defer raising an error until the module is actually used.
     """
 
-    def __init__(self, name: str, msg: Optional[str] = None):
+    def __init__(self, name: str, message: Optional[str] = None):
+        """Initializes a MissingModulePlaceholder.
+
+        Example usage:
+
+        ```python
+        from clementine import importing
+
+        try:
+            import spacy
+        except ImportError:
+            spacy = importing.MissingModulePlaceholder("spacy")
+        ```
+
+        Args:
+          name: The name of the package.
+          message: An error message.
+        """
         self._name = name
-        self._msg = msg or (
+        self._message = message or (
             f"The package {name} is not installed. Install it with "
             f"`pip install {name}`."
         )
 
     def __getattr__(self, *args, **kwargs):
-        """Raises an error when an attribute is accessed."""
-        raise errors.NotInstalledError(self._name, self._msg)
+        """Raises a ModuleNotFoundError when an attribute is accessed."""
+        raise ModuleNotFoundError(self._message)
 
     def __call__(self, *args, **kwargs):
-        """Raises an error when the object is called."""
-        raise errors.NotInstalledError(self._name, self._msg)
+        """Raises a ModuleNotFoundError when the object is called."""
+        raise ModuleNotFoundError(self._message)
 
 
 def maybe_import_module(
-    name: str, error_message: Optional[str] = None
+    name: str, message: Optional[str] = None
 ) -> Union[ModuleType, MissingModulePlaceholder]:
     """Tries to import a module by name and return it. If the module can't be
     imported, a placeholder object is returned instead.
 
+    Example usage:
+
+    ```python
+    from clementine import importing
+
+    spacy = importing.maybe_import_module("spacy")
+    ```
+
     Args:
-        name: The name of the module to import.
-        error_message: An error message to pass to the placeholder object.
+      name: The name of the module to import.
+      message: An error message to pass to the placeholder object.
     """
     try:
         return importlib.import_module(name)
     except ImportError:
-        return MissingModulePlaceholder(name, error_message)
+        return MissingModulePlaceholder(name, message)
```

### Comparing `clementine-2023.8.24/src/clementine/screenshot.py` & `clementine-2024.4.6/src/clementine/screenshot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Screenshot utilities."""
 
 import asyncio
 import os
-from typing import Optional
+from typing import Any, Optional
 
 from clementine import env, importing
 
 __all__ = ["async_screenshot", "screenshot"]
 
 _PLAYWRIGHT_IMPORT_ERROR_MESSAGE = (
     "The Playwright Python package is not installed. Install it with "
@@ -24,38 +24,74 @@
 
 async def async_screenshot(
     url: str,
     *,
     output_dir: Optional[str] = None,
     filename: Optional[str] = None,
     full_page: bool = False,
+    **kwargs: Optional[dict[str, Any]],
+) -> list[str]:
+    """Asynchronously take screenshots of a webpage in light and dark mode."""
+    output_dir = output_dir or os.path.join(os.getcwd(), "screenshots")
+    filename = filename or "screenshot"
+    color_schemes = ("light", "dark")
+    output_paths = []
+
+    async with pw_async_api.async_playwright() as p:
+        try:
+            browser = await p.webkit.launch()
+        except pw_api_types.Error as e:
+            raise OSError(
+                "The browser could not be launched. Install the Playwright "
+                "browser dependencies with `playwright install webkit`."
+            ) from e
+
+        page = await browser.new_page()
+        await page.goto(url)
+
+        os.makedirs(output_dir, exist_ok=True)
+        for color_scheme in color_schemes:
+            await page.emulate_media(color_scheme=color_scheme)
+            path = os.path.join(output_dir, f"{filename}-{color_scheme}.png")
+            await page.screenshot(path=path, full_page=full_page, **kwargs)
+            output_paths.append(path)
+
+        await browser.close()
+
+    return output_paths
+
+
+def screenshot(
+    url: str,
+    *,
+    output_dir: Optional[str] = None,
+    filename: Optional[str] = None,
+    full_page: bool = False,
+    **kwargs: Optional[dict[str, Any]],
 ) -> list[str]:
     """Take screenshots of a webpage in light and dark mode.
 
-    Use `screenshot.async_screenshot()` in asynchronous contexts, such as in a Jupyter
-    notebook. Use `screenshot.screenshot()` in synchronous contexts, such as in a
-    synchronous Python script.
+    Use `screenshot.async_screenshot()` in asynchronous contexts, such as in a
+    Jupyter notebook. Use `screenshot.screenshot()` in synchronous contexts,
+    such as in a synchronous Python script.
 
-    **Prerequisites**:
+    Prerequisites:
 
     1. Install the Playwright Python package: `pip install playwright`.
     2. Install the Playwright browser dependencies: `playwright install webkit`.
 
-
-    **Example usage**:
-
-    In a Python script:
+    Example usage in a Python script:
 
     ```python
     from clementine import screenshot
 
     paths = screenshot.screenshot('https://example.com')
     ```
 
-    In a Jupyter notebook or other asynchronous context:
+    Example usage in a Jupyter notebook or other asynchronous context:
 
     ```python
     from clementine import screenshot
     from IPython.display import display, Image
 
     paths = await screenshot.async_screenshot('https://example.com')
     for path in paths:
@@ -67,64 +103,30 @@
         https:// or file:///.
       output_dir: The directory to save the screenshots to. Defaults to
         'screenshots' in the current working directory.
       filename: The base filename to use for the screenshots. Defaults to
         'screenshot'. The screenshots will be saved as screenshot-light.png and
         screenshot-dark.png, for example.
       full_page: Whether to take a screenshot of the full page. Defaults to False.
+      **kwargs: Extra arguments to `playwright.async_api.Page.screenshot`. See
+        playwright's documentation for all possible arguments:
+        <https://playwright.dev/docs/api/class-page#page-screenshot>
 
     Raises:
       ImportError: If the Playwright Python package is not installed.
       Error: If the browser cannot be launched or an invalid url is provided.
+      RuntimeError: If called in an asynchronous context.
 
     Returns:
       A list of the paths to the screenshots.
     """
-    output_dir = output_dir or os.path.join(os.getcwd(), "screenshots")
-    filename = filename or "screenshot"
-    output_paths = []
-
-    async with pw_async_api.async_playwright() as p:
-        try:
-            browser = await p.webkit.launch()
-        except pw_api_types.Error as e:
-            raise OSError(
-                "The browser could not be launched. Install the Playwright "
-                "browser dependencies with `playwright install webkit`."
-            ) from e
-
-        page = await browser.new_page()
-        await page.goto(url)
-
-        os.makedirs(output_dir, exist_ok=True)
-        for color_scheme in ("light", "dark"):
-            await page.emulate_media(color_scheme=color_scheme)
-            path = os.path.join(output_dir, f"{filename}-{color_scheme}.png")
-            await page.screenshot(path=path, full_page=full_page)
-            output_paths.append(path)
-
-        await browser.close()
-
-    return output_paths
-
-
-def screenshot(
-    url: str,
-    *,
-    output_dir: Optional[str] = None,
-    filename: Optional[str] = None,
-    full_page=False,
-) -> list[str]:
-    """Runs the coroutine function `screenshot.async_screenshot()` and returns its
-    results."""
-    screenshot.__doc__ = async_screenshot.__doc__
     if env.is_notebook():
         raise RuntimeError(
             "The function `screenshot.screenshot()` cannot be called in "
             "an asynchronous context, such as in a Jupyter notebook. "
             "Use `screenshot.async_screenshot()` instead."
         )
     return asyncio.run(
         async_screenshot(
-            url, output_dir=output_dir, filename=filename, full_page=full_page
+            url, output_dir=output_dir, filename=filename, full_page=full_page, **kwargs
         )
     )
```

### Comparing `clementine-2023.8.24/src/clementine.egg-info/SOURCES.txt` & `clementine-2024.4.6/src/clementine.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/clementine/__init__.py
 src/clementine/__main__.py
 src/clementine/env.py
-src/clementine/errors.py
 src/clementine/importing.py
 src/clementine/py.typed
 src/clementine/screenshot.py
 src/clementine.egg-info/PKG-INFO
 src/clementine.egg-info/SOURCES.txt
 src/clementine.egg-info/dependency_links.txt
 src/clementine.egg-info/entry_points.txt
 src/clementine.egg-info/requires.txt
 src/clementine.egg-info/top_level.txt
 src/clementine/about/__init__.py
 src/clementine/about/dependencies.py
 src/clementine/cli/__init__.py
 src/clementine/cli/commands/__init__.py
 src/clementine/cli/commands/_info.py
-src/clementine/cli/commands/_screenshot.py
-tests/test_env.py
-tests/test_importing.py
-tests/test_screenshot.py
+src/clementine/cli/commands/_screenshot.py
```

### Comparing `clementine-2023.8.24/src/clementine.egg-info/requires.txt` & `clementine-2024.4.6/src/clementine.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 [blossom]
 bokeh
 gradio
 playwright
 
 [fruit]
 catppuccin-matplotlib
+keras>=3
 numpy
 pandas
 scikit-learn
+torch>=2
 
 [leaves]
+mkdocs-click
 mkdocs-walt
 mkdocstrings[python]
 
 [pulp]
 datasets
 spacy
 transformers
@@ -45,17 +48,20 @@
 rich
 
 [tree]
 bokeh
 gradio
 playwright
 catppuccin-matplotlib
+keras>=3
 numpy
 pandas
 scikit-learn
+torch>=2
+mkdocs-click
 mkdocs-walt
 mkdocstrings[python]
 datasets
 spacy
 transformers
 wandb
 build
```

