# Comparing `tmp/beaupy-3.8.1.tar.gz` & `tmp/beaupy-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaupy-3.8.1.tar", max compression
+gzip compressed data, was "beaupy-3.8.2.tar", max compression
```

## Comparing `beaupy-3.8.1.tar` & `beaupy-3.8.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1111 2024-03-27 20:15:00.094903 beaupy-3.8.1/LICENSE
--rw-r--r--   0        0        0     8094 2024-03-27 20:15:00.094903 beaupy-3.8.1/README.md
--rw-r--r--   0        0        0      260 2024-03-27 20:15:00.094903 beaupy-3.8.1/beaupy/__init__.py
--rwxr-xr-x   0        0        0    22163 2024-03-27 20:15:00.094903 beaupy-3.8.1/beaupy/_beaupy.py
--rw-r--r--   0        0        0     9315 2024-03-27 20:15:00.094903 beaupy-3.8.1/beaupy/_internals.py
--rw-r--r--   0        0        0      170 2024-03-27 20:15:00.094903 beaupy-3.8.1/beaupy/spinners/__init__.py
--rw-r--r--   0        0        0     2335 2024-03-27 20:15:00.094903 beaupy-3.8.1/beaupy/spinners/_spinners.py
--rw-r--r--   0        0        0     3704 2024-03-27 20:15:00.098903 beaupy-3.8.1/pyproject.toml
--rw-r--r--   0        0        0     9169 1970-01-01 00:00:00.000000 beaupy-3.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-04-06 17:20:39.647693 beaupy-3.8.2/LICENSE
+-rw-r--r--   0        0        0     8094 2024-04-06 17:20:39.647693 beaupy-3.8.2/README.md
+-rw-r--r--   0        0        0      260 2024-04-06 17:20:39.647693 beaupy-3.8.2/beaupy/__init__.py
+-rwxr-xr-x   0        0        0    22165 2024-04-06 17:20:39.647693 beaupy-3.8.2/beaupy/_beaupy.py
+-rw-r--r--   0        0        0     9315 2024-04-06 17:20:39.647693 beaupy-3.8.2/beaupy/_internals.py
+-rw-r--r--   0        0        0      170 2024-04-06 17:20:39.651693 beaupy-3.8.2/beaupy/spinners/__init__.py
+-rw-r--r--   0        0        0     2335 2024-04-06 17:20:39.651693 beaupy-3.8.2/beaupy/spinners/_spinners.py
+-rw-r--r--   0        0        0     3704 2024-04-06 17:20:39.651693 beaupy-3.8.2/pyproject.toml
+-rw-r--r--   0        0        0     9169 1970-01-01 00:00:00.000000 beaupy-3.8.2/PKG-INFO
```

### Comparing `beaupy-3.8.1/LICENSE` & `beaupy-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beaupy-3.8.1/README.md` & `beaupy-3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `beaupy-3.8.1/beaupy/_beaupy.py` & `beaupy-3.8.2/beaupy/_beaupy.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         if Config.raise_on_interrupt:
             raise KeyboardInterrupt()
         state.abort = True
 
     elif any([keypress in navigation_keys for navigation_keys in _navigation_keys]):
         state = _navigate_select(state, keypress=keypress)
     elif keypress in DefaultKeys.select_all:
-        if len(state.selected_indexes) == maximal_count if maximal_count is not None else len(state.options):
+        if len(state.selected_indexes) == (maximal_count if maximal_count is not None else len(state.options)):
             state.selected_indexes = []
         else:
             if maximal_count is not None:
                 state.selected_indexes = list(range(maximal_count))
                 state.error = f'Must select at most {maximal_count} options'
             else:
                 state.selected_indexes = list(range(len(state.options)))
```

### Comparing `beaupy-3.8.1/beaupy/_internals.py` & `beaupy-3.8.2/beaupy/_internals.py`

 * *Files identical despite different names*

### Comparing `beaupy-3.8.1/beaupy/spinners/_spinners.py` & `beaupy-3.8.2/beaupy/spinners/_spinners.py`

 * *Files identical despite different names*

### Comparing `beaupy-3.8.1/pyproject.toml` & `beaupy-3.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'beaupy'
-version = '3.8.1'
+version = '3.8.2'
 description = 'A library of elements for interactive TUIs in Python'
 authors = ['Peter Vyboch <pvyboch1@gmail.com>']
 license = 'MIT'
 repository = 'https://github.com/petereon/beaupy'
 readme = 'README.md'
 keywords = ["cli", "interactive", "console", "terminal", "interface"]
 classifiers = [
```

### Comparing `beaupy-3.8.1/PKG-INFO` & `beaupy-3.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaupy
-Version: 3.8.1
+Version: 3.8.2
 Summary: A library of elements for interactive TUIs in Python
 Home-page: https://github.com/petereon/beaupy
 License: MIT
 Keywords: cli,interactive,console,terminal,interface
 Author: Peter Vyboch
 Author-email: pvyboch1@gmail.com
 Requires-Python: >=3.7.8,<4.0.0
```

