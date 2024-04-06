# Comparing `tmp/dargs-0.4.4.tar.gz` & `tmp/dargs-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/dargs/dargs/dist/.tmp-3vlzekni/dargs-0.4.4.tar", last modified: Wed Feb 21 07:53:51 2024, max compression
+gzip compressed data, was "/home/runner/work/dargs/dargs/dist/.tmp-3umrb0v1/dargs-0.4.5.tar", last modified: Sat Apr  6 04:45:34 2024, max compression
```

## Comparing `dargs-0.4.4.tar` & `dargs-0.4.5.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:53:51.000000 dargs-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:53:51.000000 dargs-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:53:51.000000 dargs-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-21 07:53:36.000000 dargs-0.4.4/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-21 07:53:36.000000 dargs-0.4.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-21 07:53:36.000000 dargs-0.4.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-21 07:53:36.000000 dargs-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-21 07:53:36.000000 dargs-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-21 07:53:36.000000 dargs-0.4.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-21 07:53:36.000000 dargs-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-02-21 07:53:51.000000 dargs-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-21 07:53:36.000000 dargs-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-21 07:53:36.000000 dargs-0.4.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:53:51.000000 dargs-0.4.4/dargs/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-21 07:53:36.000000 dargs-0.4.4/dargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-21 07:53:51.000000 dargs-0.4.4/dargs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    36996 2024-02-21 07:53:36.000000 dargs-0.4.4/dargs/dargs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-02-21 07:53:36.000000 dargs-0.4.4/dargs/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-02-21 07:53:36.000000 dargs-0.4.4/dargs/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:53:51.000000 dargs-0.4.4/dargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-02-21 07:53:51.000000 dargs-0.4.4/dargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-21 07:53:51.000000 dargs-0.4.4/dargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 07:53:51.000000 dargs-0.4.4/dargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-21 07:53:51.000000 dargs-0.4.4/dargs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-21 07:53:51.000000 dargs-0.4.4/dargs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:53:51.000000 dargs-0.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-21 07:53:36.000000 dargs-0.4.4/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-21 07:53:36.000000 dargs-0.4.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-02-21 07:53:36.000000 dargs-0.4.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-21 07:53:36.000000 dargs-0.4.4/docs/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-21 07:53:36.000000 dargs-0.4.4/docs/dpgui.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-21 07:53:36.000000 dargs-0.4.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-21 07:53:36.000000 dargs-0.4.4/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-02-21 07:53:36.000000 dargs-0.4.4/docs/nb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-21 07:53:36.000000 dargs-0.4.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-21 07:53:36.000000 dargs-0.4.4/docs/sphinx.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-02-21 07:53:36.000000 dargs-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 07:53:51.000000 dargs-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:53:51.000000 dargs-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-21 07:53:36.000000 dargs-0.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 07:53:36.000000 dargs-0.4.4/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    38837 2024-02-21 07:53:36.000000 dargs-0.4.4/tests/dpmdargs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-02-21 07:53:36.000000 dargs-0.4.4/tests/test_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-02-21 07:53:36.000000 dargs-0.4.4/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-02-21 07:53:36.000000 dargs-0.4.4/tests/test_docgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-02-21 07:53:36.000000 dargs-0.4.4/tests/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-02-21 07:53:36.000000 dargs-0.4.4/tests/test_notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-06 04:45:16.000000 dargs-0.4.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-06 04:45:16.000000 dargs-0.4.5/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-06 04:45:16.000000 dargs-0.4.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-06 04:45:16.000000 dargs-0.4.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-06 04:45:16.000000 dargs-0.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-06 04:45:16.000000 dargs-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-06 04:45:16.000000 dargs-0.4.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-06 04:45:16.000000 dargs-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-06 04:45:34.000000 dargs-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-06 04:45:16.000000 dargs-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-06 04:45:16.000000 dargs-0.4.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/dargs/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-06 04:45:16.000000 dargs-0.4.5/dargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37717 2024-04-06 04:45:16.000000 dargs-0.4.5/dargs/dargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-06 04:45:16.000000 dargs-0.4.5/dargs/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-06 04:45:16.000000 dargs-0.4.5/dargs/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/dargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/dpgui.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/nb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-06 04:45:16.000000 dargs-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 04:45:34.000000 dargs-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38837 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/dpmdargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/test_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/test_docgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/test_notebook.py
```

### Comparing `dargs-0.4.4/.github/workflows/python-publish.yml` & `dargs-0.4.5/.github/workflows/python-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - name: Get history and tags for SCM versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: 3.7
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build twine
     - name: Build and publish
```

### Comparing `dargs-0.4.4/.gitignore` & `dargs-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/.pre-commit-config.yaml` & `dargs-0.4.5/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     -   id: check-json
     -   id: check-added-large-files
     -   id: check-merge-conflict
     -   id: check-symlinks
     -   id: check-toml
 # Python
 -   repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.2
+    rev: v0.3.5
     hooks:
     - id: ruff
       args: [ --fix ]
     - id: ruff-format
 # numpydoc
 -   repo: https://github.com/Carreau/velin
     rev: 0.0.12
```

### Comparing `dargs-0.4.4/.readthedocs.yaml` & `dargs-0.4.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/LICENSE` & `dargs-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/PKG-INFO` & `dargs-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargs
-Version: 0.4.4
+Version: 0.4.5
 Summary: Process arguments for the deep modeling project.
 Author: DeepModeling
 Author-email: Yixiao Chen <yixiaoc@princeton.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `dargs-0.4.4/README.md` & `dargs-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/dargs/dargs.py` & `dargs-0.4.5/dargs/dargs.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 `sub_variants` to mimic the union behavior in the type structure.
 
 Due to the complexity of *Variant* structure, it is implemented into a
 separate class `Variant` so that multiple choices can be handled correctly.
 We also need to pay special attention to flat the keys of its choices.
 """
 
-
+import difflib
 import fnmatch
 import json
 import re
 from copy import deepcopy
 from enum import Enum
 from textwrap import indent
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
@@ -461,16 +461,18 @@
         allowed_keys = self.flatten_sub(value, path).keys()
         # curpath = [*path, self.name]
         if not len(allowed_keys):
             # no allowed keys defined, allow any keys
             return
         for name in value.keys():
             if name not in allowed_keys:
+                dym_message = did_you_mean(name, allowed_keys)
                 raise ArgumentKeyError(
-                    path, f"undefined key `{name}` is " "not allowed in strict mode"
+                    path,
+                    f"undefined key `{name}` is not allowed in strict mode. {dym_message}",
                 )
 
     # above are type checking part
     # below are normalizing part
 
     def normalize(
         self,
@@ -797,15 +799,20 @@
             tag = argdict[self.flag_name]
             if tag in self.choice_dict:
                 return self.choice_dict[tag]
             elif tag in self.choice_alias:
                 return self.choice_dict[self.choice_alias[tag]]
             else:
                 raise ArgumentValueError(
-                    path, f"get invalid choice `{tag}` for flag key `{self.flag_name}`."
+                    path,
+                    f"get invalid choice `{tag}` for flag key `{self.flag_name}`."
+                    + did_you_mean(
+                        tag,
+                        list(self.choice_dict.keys()) + list(self.choice_alias.keys()),
+                    ),
                 )
         elif self.optional:
             return self.choice_dict[self.default_tag]
         else:
             raise ArgumentKeyError(
                 path,
                 f"key `{self.flag_name}` is required "
@@ -1039,7 +1046,26 @@
                 "doc": obj.doc,
             }
         elif isinstance(get_origin(obj), type):
             return get_origin(obj).__name__
         elif isinstance(obj, type):
             return obj.__name__
         return json.JSONEncoder.default(self, obj)
+
+
+def did_you_mean(choice: str, choices: List[str]) -> str:
+    """Get did you mean message.
+
+    Parameters
+    ----------
+    choice : str
+        the user's wrong choice
+    choices : list[str]
+        all the choices
+
+    Returns
+    -------
+    str
+        did you mean error message
+    """
+    matches = difflib.get_close_matches(choice, choices)
+    return f"Did you mean: {matches[0]}?" if matches else ""
```

### Comparing `dargs-0.4.4/dargs/notebook.py` & `dargs-0.4.5/dargs/notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,14 +294,18 @@
             if not _last_one:
                 buff.append(",")
             buff.append("</code>")
             buff.append(linebreak)
         else:
             buff.append(r"""<code class="dargs-code">""")
             buff.append(
-                json.dumps(self.data, indent=2).replace("\n", f"{linebreak}{indent}")
+                json.dumps(self.data, indent=2)
+                .replace(" ", "&nbsp;")
+                .replace(
+                    "\n", f"""</code>{linebreak}{indent}<code class="dargs-code">"""
+                )
             )
             if not _last_one:
                 buff.append(",")
             buff.append("</code>")
             buff.append(linebreak)
         return "".join(buff)
```

### Comparing `dargs-0.4.4/dargs/sphinx.py` & `dargs-0.4.5/dargs/sphinx.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     .. dargs::
        :module: dargs.sphinx
        :func: _test_argument
 
 where `_test_argument` returns an :class:`Argument <dargs.Argument>`. A :class:`list` of :class:`Argument <dargs.Argument>` is also accepted.
 """
+
 import sys
 from typing import ClassVar, List
 
 from docutils.parsers.rst import Directive
 from docutils.parsers.rst.directives import unchanged
 from sphinx import addnodes
 from sphinx.directives import ObjectDescription
@@ -166,14 +167,15 @@
     doc_test = "This argument/variant is only used to test."
     return Argument(
         name="test",
         dtype=str,
         doc=doc_test,
         sub_fields=[
             Argument("test_argument", dtype=str, doc=doc_test, default="test"),
+            Argument("test_list", dtype=List[int], optional=True),
         ],
         sub_variants=[
             Variant(
                 "test_variant",
                 doc=doc_test,
                 choices=[
                     Argument(
```

### Comparing `dargs-0.4.4/dargs.egg-info/PKG-INFO` & `dargs-0.4.5/dargs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargs
-Version: 0.4.4
+Version: 0.4.5
 Summary: Process arguments for the deep modeling project.
 Author: DeepModeling
 Author-email: Yixiao Chen <yixiaoc@princeton.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `dargs-0.4.4/dargs.egg-info/SOURCES.txt` & `dargs-0.4.5/dargs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 README.md
 codecov.yml
 pyproject.toml
+.github/dependabot.yml
 .github/workflows/mirror_gitee.yml
 .github/workflows/python-publish.yml
 .github/workflows/test.yml
 dargs/__init__.py
 dargs/_version.py
 dargs/dargs.py
 dargs/notebook.py
```

### Comparing `dargs-0.4.4/docs/Makefile` & `dargs-0.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/docs/conf.py` & `dargs-0.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/docs/dpgui.rst` & `dargs-0.4.5/docs/dpgui.rst`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/docs/intro.md` & `dargs-0.4.5/docs/intro.md`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/docs/nb.ipynb` & `dargs-0.4.5/docs/nb.ipynb`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989583333333334%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(6, \'    "test_list": [\\n\'), (7, \'        1,\\n\'), '*

 * *            "(8, '        2,\\n'), (9, '        3\\n'), (10, '    ],\\n')]}}}"}*

```diff
@@ -17,14 +17,19 @@
             "source": [
                 "from dargs.sphinx import _test_argument\n",
                 "from dargs.notebook import JSON\n",
                 "\n",
                 "jstr = \"\"\"\n",
                 "{\n",
                 "    \"test_argument\": \"test1\",\n",
+                "    \"test_list\": [\n",
+                "        1,\n",
+                "        2,\n",
+                "        3\n",
+                "    ],\n",
                 "    \"test_variant\": \"test_variant_argument\",\n",
                 "    \"test_repeat\": [\n",
                 "        {\"test_repeat_item\": false},\n",
                 "        {\"test_repeat_item\": true}\n",
                 "    ],\n",
                 "    \"_comment\": \"This is an example data\"\n",
                 "}\n",
```

### Comparing `dargs-0.4.4/docs/sphinx.rst` & `dargs-0.4.5/docs/sphinx.rst`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/pyproject.toml` & `dargs-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/tests/dpmdargs.py` & `dargs-0.4.5/tests/dpmdargs.py`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/tests/test_checker.py` & `dargs-0.4.5/tests/test_checker.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,16 +84,17 @@
         err_dict1 = {
             "base": {"sub1": 1, "sub2": {"subsub1": 11, "subsub2": {"subsubsub2": 111}}}
         }  # different name here
         with self.assertRaises(ArgumentKeyError):
             ca.check(err_dict1)
         err_dict1["base"]["sub2"]["subsub2"]["subsubsub1"] = 111
         ca.check(err_dict1)  # now should pass
-        with self.assertRaises(ArgumentKeyError):
+        with self.assertRaises(ArgumentKeyError) as cm:
             ca.check(err_dict1, strict=True)  # but should fail when strict
+        self.assertIn("Did you mean: subsubsub1?", str(cm.exception))
         err_dict1["base"]["sub2"] = None
         with self.assertRaises(ArgumentTypeError):
             ca.check(err_dict1)
         # make sure no dup keys is allowed
         with self.assertRaises(ValueError):
             Argument("base", dict, [Argument("sub1", int), Argument("sub1", int)])
 
@@ -245,16 +246,17 @@
                 "sub1": 1,
                 "sub2": "a",
                 "vnt_flag": "badtype",  # here is wrong
                 "shared": 20,
                 "vnt2_1": 21,
             }
         }
-        with self.assertRaises(ArgumentValueError):
+        with self.assertRaises(ArgumentValueError) as cm:
             ca.check(err_dict2)
+        self.assertIn("Did you mean: type3?", str(cm.exception))
         # test optional choice
         test_dict1["base"].pop("vnt_flag")
         with self.assertRaises(ArgumentKeyError):
             ca.check(test_dict1)
         ca.sub_variants["vnt_flag"].optional = True
         ca.sub_variants["vnt_flag"].default_tag = "type1"
         ca.check(test_dict1)
```

### Comparing `dargs-0.4.4/tests/test_creation.py` & `dargs-0.4.5/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/tests/test_docgen.py` & `dargs-0.4.5/tests/test_docgen.py`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/tests/test_normalizer.py` & `dargs-0.4.5/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `dargs-0.4.4/tests/test_notebook.py` & `dargs-0.4.5/tests/test_notebook.py`

 * *Files identical despite different names*

