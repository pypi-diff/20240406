# Comparing `tmp/earthdata-varinfo-2.2.0.tar.gz` & `tmp/earthdata-varinfo-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthdata-varinfo-2.2.0.tar", last modified: Mon Dec  4 22:18:12 2023, max compression
+gzip compressed data, was "earthdata-varinfo-2.2.1.tar", last modified: Sat Apr  6 16:44:10 2024, max compression
```

## Comparing `earthdata-varinfo-2.2.0.tar` & `earthdata-varinfo-2.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 22:18:12.209070 earthdata-varinfo-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2023-12-04 22:18:12.209070 earthdata-varinfo-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 22:18:12.205070 earthdata-varinfo-2.2.0/earthdata_varinfo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2023-12-04 22:18:12.000000 earthdata-varinfo-2.2.0/earthdata_varinfo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-12-04 22:18:12.000000 earthdata-varinfo-2.2.0/earthdata_varinfo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 22:18:12.000000 earthdata-varinfo-2.2.0/earthdata_varinfo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-04 22:18:12.000000 earthdata-varinfo-2.2.0/earthdata_varinfo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-04 22:18:12.000000 earthdata-varinfo-2.2.0/earthdata_varinfo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 22:18:12.209070 earthdata-varinfo-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 22:18:12.205070 earthdata-varinfo-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/tests/test_code_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 22:18:12.205070 earthdata-varinfo-2.2.0/varinfo/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/varinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/varinfo/cf_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/varinfo/cmr_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/varinfo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/varinfo/generate_umm_var.py
--rw-r--r--   0 runner    (1001) docker     (127)    16800 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/varinfo/umm_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/varinfo/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    27256 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/varinfo/var_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    19766 2023-12-04 22:17:57.000000 earthdata-varinfo-2.2.0/varinfo/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:44:10.256742 earthdata-varinfo-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-06 16:44:10.252742 earthdata-varinfo-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:44:10.252742 earthdata-varinfo-2.2.1/earthdata_varinfo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-06 16:44:10.000000 earthdata-varinfo-2.2.1/earthdata_varinfo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-06 16:44:10.000000 earthdata-varinfo-2.2.1/earthdata_varinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:44:10.000000 earthdata-varinfo-2.2.1/earthdata_varinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-06 16:44:10.000000 earthdata-varinfo-2.2.1/earthdata_varinfo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 16:44:10.000000 earthdata-varinfo-2.2.1/earthdata_varinfo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:44:10.256742 earthdata-varinfo-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:44:10.252742 earthdata-varinfo-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/tests/test_code_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:44:10.252742 earthdata-varinfo-2.2.1/varinfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/varinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/varinfo/cf_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/varinfo/cmr_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/varinfo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/varinfo/generate_umm_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16291 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/varinfo/umm_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/varinfo/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26436 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/varinfo/var_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-04-06 16:43:58.000000 earthdata-varinfo-2.2.1/varinfo/variable.py
```

### Comparing `earthdata-varinfo-2.2.0/CHANGELOG.md` & `earthdata-varinfo-2.2.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v2.2.1
+### Unreleased
+
+The `requests` package has been added as an explicit dependency of the package.
+Additionally, black code formatting has been applied to the entire repository.
+
 ## v2.2.0
 ### 2023-11-30
 
 This version of `earthdata-varinfo` updates `varinfo.cmr_search` to include
 functionality to get a users EDL token given a LaunchPad token with
 `get_edl_token_from_launchpad` and `get_edl_token_header`.
 `get_edl_token_from_launchpad` returns a users EDL token given a LaunchPad
```

### Comparing `earthdata-varinfo-2.2.0/LICENSE` & `earthdata-varinfo-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `earthdata-varinfo-2.2.0/PKG-INFO` & `earthdata-varinfo-2.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: earthdata-varinfo
-Version: 2.2.0
-Summary: A package for parsing Earth Observation science granule structure and extracting relations between science variables and their associated metadata, such as coordinates.
-Home-page: https://github.com/nasa/earthdata-varinfo
-Author: NASA EOSDIS SDPS Data Services Team
-Author-email: owen.m.littlejohns@nasa.gov
-License: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: netCDF4~=1.6.3
-Requires-Dist: numpy~=1.24.2
-Requires-Dist: python-cmr~=0.9.0
-Provides-Extra: dev
-Requires-Dist: coverage~=5.5; extra == "dev"
-Requires-Dist: ipython~=8.0.1; extra == "dev"
-Requires-Dist: jsonschema~=4.17.3; extra == "dev"
-Requires-Dist: pycodestyle~=2.11.0; extra == "dev"
-Requires-Dist: pylint>=2.5.0; extra == "dev"
-Requires-Dist: unittest-xml-reporting~=3.0.4; extra == "dev"
-
 # earthdata-varinfo
 
 A Python package developed as part of the NASA Earth Observing System Data and
 Information System (EOSDIS) for parsing Earth Observation science granule
 structure and extracting relations between science variables and their
 associated metadata, such as coordinates. This package also includes the
 capability to generate variable (UMM-Var) metadata records that are compatible
@@ -227,14 +202,47 @@
 
 Run `unittest` suite:
 
 ```bash
 $ make test
 ```
 
+### pre-commit hooks:
+
+This repository uses [pre-commit](https://pre-commit.com/) to enable pre-commit
+checking the repository for some coding standard best practices. These include:
+
+* Removing trailing whitespaces.
+* Removing blank lines at the end of a file.
+* JSON files have valid formats.
+* [ruff](https://github.com/astral-sh/ruff) Python linting checks.
+* [black](https://black.readthedocs.io/en/stable/index.html) Python code
+  formatting checks.
+
+To enable these checks:
+
+```bash
+# Install pre-commit Python package as part of test requirements:
+pip install -r dev-requirements.txt
+
+# Install the git hook scripts:
+pre-commit install
+
+# (Optional) Run against all files:
+pre-commit run --all-files
+```
+
+When you try to make a new commit locally, `pre-commit` will automatically run.
+If any of the hooks detect non-compliance (e.g., trailing whitespace), that
+hook will state it failed, and also try to fix the issue. You will need to
+review and `git add` the changes before you can make a commit.
+
+It is planned to implement additional hooks, possibly including tools such as
+`mypy`.
+
 ## Releasing:
 
 All CI/CD for this repository is defined in the `.github/workflows` directory:
 
 * run_tests.yml - A reusable workflow that runs the unit test suite under a
   matrix of Python versions.
 * run_tests_on_pull_requests.yml - Triggered for all PRs against main. It runs
```

### Comparing `earthdata-varinfo-2.2.0/earthdata_varinfo.egg-info/PKG-INFO` & `earthdata-varinfo-2.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: earthdata-varinfo
-Version: 2.2.0
+Version: 2.2.1
 Summary: A package for parsing Earth Observation science granule structure and extracting relations between science variables and their associated metadata, such as coordinates.
 Home-page: https://github.com/nasa/earthdata-varinfo
 Author: NASA EOSDIS SDPS Data Services Team
 Author-email: owen.m.littlejohns@nasa.gov
 License: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: netCDF4~=1.6.3
 Requires-Dist: numpy~=1.24.2
 Requires-Dist: python-cmr~=0.9.0
+Requires-Dist: requests~=2.31.0
 Provides-Extra: dev
 Requires-Dist: coverage~=5.5; extra == "dev"
 Requires-Dist: ipython~=8.0.1; extra == "dev"
 Requires-Dist: jsonschema~=4.17.3; extra == "dev"
+Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 Requires-Dist: pycodestyle~=2.11.0; extra == "dev"
 Requires-Dist: pylint>=2.5.0; extra == "dev"
 Requires-Dist: unittest-xml-reporting~=3.0.4; extra == "dev"
 
 # earthdata-varinfo
 
 A Python package developed as part of the NASA Earth Observing System Data and
@@ -227,14 +229,47 @@
 
 Run `unittest` suite:
 
 ```bash
 $ make test
 ```
 
+### pre-commit hooks:
+
+This repository uses [pre-commit](https://pre-commit.com/) to enable pre-commit
+checking the repository for some coding standard best practices. These include:
+
+* Removing trailing whitespaces.
+* Removing blank lines at the end of a file.
+* JSON files have valid formats.
+* [ruff](https://github.com/astral-sh/ruff) Python linting checks.
+* [black](https://black.readthedocs.io/en/stable/index.html) Python code
+  formatting checks.
+
+To enable these checks:
+
+```bash
+# Install pre-commit Python package as part of test requirements:
+pip install -r dev-requirements.txt
+
+# Install the git hook scripts:
+pre-commit install
+
+# (Optional) Run against all files:
+pre-commit run --all-files
+```
+
+When you try to make a new commit locally, `pre-commit` will automatically run.
+If any of the hooks detect non-compliance (e.g., trailing whitespace), that
+hook will state it failed, and also try to fix the issue. You will need to
+review and `git add` the changes before you can make a commit.
+
+It is planned to implement additional hooks, possibly including tools such as
+`mypy`.
+
 ## Releasing:
 
 All CI/CD for this repository is defined in the `.github/workflows` directory:
 
 * run_tests.yml - A reusable workflow that runs the unit test suite under a
   matrix of Python versions.
 * run_tests_on_pull_requests.yml - Triggered for all PRs against main. It runs
```

### Comparing `earthdata-varinfo-2.2.0/earthdata_varinfo.egg-info/SOURCES.txt` & `earthdata-varinfo-2.2.1/earthdata_varinfo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthdata-varinfo-2.2.0/setup.py` & `earthdata-varinfo-2.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,76 @@
 """ Scaffolding for the earthdata-varinfo package
 
     Note: license and classifier list:
     https://pypi.org/pypi?%3Aaction=list_classifiers
 
 """
+
 from typing import List
 import io
 import pathlib
 import os
 
 from setuptools import find_packages, setup
 
 
 CURRENT_DIRECTORY = pathlib.Path(__file__).parent.resolve()
 
 
 def parse_dependencies(file_path: str) -> List[str]:
-    """ Parse a Pip requirements file, and extract the dependencies. """
+    """Parse a Pip requirements file, and extract the dependencies."""
     with open(file_path, 'r') as file_handler:
         dependencies = file_handler.read().strip().split('\n')
 
     return dependencies
 
 
 def get_readme(current_directory: str) -> str:
-    """ Parse the README.md in the root of the repository, for the long
-        description of this Python package.
+    """Parse the README.md in the root of the repository, for the long
+    description of this Python package.
 
     """
-    with io.open(os.path.join(current_directory, 'README.md'),
-                 'r', encoding='utf-8') as file_handler:
+    with io.open(
+        os.path.join(current_directory, 'README.md'), 'r', encoding='utf-8'
+    ) as file_handler:
         readme = file_handler.read()
 
     return readme
 
 
 def get_semantic_version(current_directory: str) -> str:
-    """ Parse the VERSION file in the root of the repository for the semantic
-        version number of the version.
+    """Parse the VERSION file in the root of the repository for the semantic
+    version number of the version.
 
     """
     with open(os.path.join(current_directory, 'VERSION'), 'r') as file_handler:
         semantic_version = file_handler.read().strip()
 
     return semantic_version
 
 
 setup(
     name='earthdata-varinfo',
     version=get_semantic_version(CURRENT_DIRECTORY),
     author='NASA EOSDIS SDPS Data Services Team',
     author_email='owen.m.littlejohns@nasa.gov',
-    description=('A package for parsing Earth Observation science granule '
-                 'structure and extracting relations between science variables'
-                 ' and their associated metadata, such as coordinates.'),
+    description=(
+        'A package for parsing Earth Observation science granule '
+        'structure and extracting relations between science variables'
+        ' and their associated metadata, such as coordinates.'
+    ),
     long_description=get_readme(CURRENT_DIRECTORY),
     long_description_content_type='text/markdown',
     url='https://github.com/nasa/earthdata-varinfo',
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     include_package_data=True,
     install_requires=parse_dependencies('requirements.txt'),
     extras_require={'dev': parse_dependencies('dev-requirements.txt')},
     test_suite='tests',
     python_requires='>=3.7',
     license='License :: OSI Approved :: Apache Software License',
-    classifiers=['Programming Language :: Python',
-                 'Programming Language :: Python :: 3',
-                 'Operating System :: OS Independent'],
+    classifiers=[
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Operating System :: OS Independent',
+    ],
 )
```

### Comparing `earthdata-varinfo-2.2.0/tests/test_code_format.py` & `earthdata-varinfo-2.2.1/tests/test_code_format.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from pathlib import Path
 from unittest import TestCase
 
 from pycodestyle import StyleGuide
 
 
 class TestCodeFormat(TestCase):
-    """ This test class should ensure all earthdata-varinfo Python code adheres
-        to standard Python code styling.
+    """This test class should ensure all earthdata-varinfo Python code adheres
+    to standard Python code styling.
 
-        Ignored errors and warnings:
-
-        * E501: Line length, which defaults to 80 characters. This is a
-                preferred feature of the code, but not always easily achieved.
-        * W503: Break before binary operator. Have to ignore one of W503 or
-                W504 to allow for breaking of some long lines. PEP8 suggests
-                breaking the line before a binary operator is more "Pythonic".
+    Ignored errors and warnings:
 
+    * E501: Line length, which defaults to 80 characters. This is a
+            preferred feature of the code, but not always easily achieved.
+    * W503: Break before binary operator. Have to ignore one of W503 or
+            W504 to allow for breaking of some long lines. PEP8 suggests
+            breaking the line before a binary operator is more "Pythonic".
+    * E203, E701: This repository uses black code formatting, which deviates
+                  from PEP8 for these errors.
     """
+
     @classmethod
     def setUpClass(cls):
         cls.python_files = Path('varinfo').rglob('*.py')
 
     def test_pycodestyle_adherence(self):
-        """ Ensure all code in the `varinfo` directory adheres to PEP8 defined
-            standards.
+        """Ensure all code in the `varinfo` directory adheres to PEP8 defined
+        standards.
 
         """
-        style_guide = StyleGuide(ignore=['E501', 'W503'])
+        style_guide = StyleGuide(ignore=['E501', 'W503', 'E203', 'E701'])
         results = style_guide.check_files(self.python_files)
         self.assertEqual(results.total_errors, 0, 'Found code style issues.')
```

### Comparing `earthdata-varinfo-2.2.0/varinfo/cf_config.py` & `earthdata-varinfo-2.2.1/varinfo/cf_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,39 +14,47 @@
     The configuration file also specifies variables that are incorrectly
     considered as science variables by the VarInfo class, due to them having
     references in the coordinates attribute. Further, there are required
     variables that have to be included in the output of any variable subset
     request for a specific collection.
 
 """
+
 from os.path import exists
 from typing import Dict, Optional
 import json
 import re
 
-from varinfo.exceptions import (InvalidConfigFileFormatError,
-                                MissingConfigurationFileError)
+from varinfo.exceptions import (
+    InvalidConfigFileFormatError,
+    MissingConfigurationFileError,
+)
 
 
 class CFConfig:
-    """ This class should read the main configuration file,
-        see e.g. sample_config.json, which defines overriding values and
-        supplements for the attributes stored in fields such as
-        ancillary_variables, or dimensions.
-
-        Given a mission and collection short name, upon instantiation, the
-        object should only retain information relevant to that specific
-        collection.
+    """This class should read the main configuration file,
+    see e.g. sample_config.json, which defines overriding values and
+    supplements for the attributes stored in fields such as
+    ancillary_variables, or dimensions.
+
+    Given a mission and collection short name, upon instantiation, the
+    object should only retain information relevant to that specific
+    collection.
 
     """
-    def __init__(self, mission: str, collection_short_name: str,
-                 config_file: Optional[str] = None):
-        """ Set supplied class attributes. Then read the designated
-            configuration file to obtain mission and short name specific
-            attributes.
+
+    def __init__(
+        self,
+        mission: str,
+        collection_short_name: str,
+        config_file: Optional[str] = None,
+    ):
+        """Set supplied class attributes. Then read the designated
+        configuration file to obtain mission and short name specific
+        attributes.
 
         """
         self.config_file = config_file
         self.mission = mission
         self.short_name = collection_short_name
 
         self._cf_overrides = {}
@@ -56,100 +64,107 @@
         self.global_supplements = {}
         self.global_overrides = {}
 
         if self.mission is not None:
             self._read_config_file()
 
     def _read_config_file(self):
-        """ Open the main configuration JSON file and extract only those parts
-            of it pertaining to the mission and collection specified upon
-            instantiating the class.
+        """Open the main configuration JSON file and extract only those parts
+        of it pertaining to the mission and collection specified upon
+        instantiating the class.
 
         """
         if self.config_file is not None and not exists(self.config_file):
             raise MissingConfigurationFileError(self.config_file)
-        elif (
-            self.config_file is not None and self.config_file.endswith('.json')
-        ):
+        elif self.config_file is not None and self.config_file.endswith('.json'):
             with open(self.config_file, 'r', encoding='utf-8') as file_handler:
                 config = json.load(file_handler)
         elif self.config_file is not None:
             raise InvalidConfigFileFormatError(self.config_file)
         else:
             config = {}
 
         self.excluded_science_variables = {
             pattern
             for item in config.get('Excluded_Science_Variables', [])
-            if self._is_applicable(item['Applicability'].get('Mission'),
-                                   item['Applicability'].get('ShortNamePath'))
+            if self._is_applicable(
+                item['Applicability'].get('Mission'),
+                item['Applicability'].get('ShortNamePath'),
+            )
             for pattern in item['Variable_Pattern']
         }
 
         self.required_variables = {
             pattern
             for item in config.get('Required_Fields', [])
-            if self._is_applicable(item['Applicability'].get('Mission'),
-                                   item['Applicability'].get('ShortNamePath'))
+            if self._is_applicable(
+                item['Applicability'].get('Mission'),
+                item['Applicability'].get('ShortNamePath'),
+            )
             for pattern in item['Variable_Pattern']
         }
 
         self.global_supplements = {
             attribute['Name']: attribute['Value']
             for item in config.get('CF_Supplements', [])
-            if self._is_applicable(item['Applicability'].get('Mission'),
-                                   item['Applicability'].get('ShortNamePath'))
+            if self._is_applicable(
+                item['Applicability'].get('Mission'),
+                item['Applicability'].get('ShortNamePath'),
+            )
             for attribute in item.get('Global_Attributes', [])
         }
 
         self.global_overrides = {
             attribute['Name']: attribute['Value']
             for item in config.get('CF_Overrides', [])
-            if self._is_applicable(item['Applicability'].get('Mission'),
-                                   item['Applicability'].get('ShortNamePath'))
+            if self._is_applicable(
+                item['Applicability'].get('Mission'),
+                item['Applicability'].get('ShortNamePath'),
+            )
             for attribute in item.get('Global_Attributes', [])
         }
 
         for override in config.get('CF_Overrides', []):
             self._process_cf_item(override, self._cf_overrides)
 
         for supplement in config.get('CF_Supplements', []):
             self._process_cf_item(supplement, self._cf_supplements)
 
     def _is_applicable(self, mission: str, short_name: str = None) -> bool:
-        """ Given a mission, and optionally also a collection short name, of an
-            applicability within the configuration file, check for a match
-            against the mission and short name specified when instantiating the
-            class object.
+        """Given a mission, and optionally also a collection short name, of an
+        applicability within the configuration file, check for a match
+        against the mission and short name specified when instantiating the
+        class object.
 
         """
         mission_matches = re.match(mission, self.mission) is not None
 
         short_name_matches = (
-            short_name is None
-            or re.match(short_name, self.short_name) is not None
+            short_name is None or re.match(short_name, self.short_name) is not None
         )
 
         return mission_matches and short_name_matches
 
-    def _process_cf_item(self,
-                         cf_item: Dict,
-                         results: Dict[str, Dict],
-                         input_mission: str = None,
-                         input_short_name: str = None):
-        """ Process a single block in the CF overrides or CF supplements region
-            of the configuration file. First check that the applicability
-            matches the mission and short name for the class. Next, check
-            for a variable pattern. This is indicative of there being
-            overriding or supplemental attributes in this list item.
-            Assign any information to the results dictionary, with a key of
-            that variable pattern. Lastly, check for any nested references,
-            which are child blocks to be processed in the same way. The mission
-            and short name from this block are passed to all children, as they
-            may not both be defined, due to assumed inheritance.
+    def _process_cf_item(
+        self,
+        cf_item: Dict,
+        results: Dict[str, Dict],
+        input_mission: str = None,
+        input_short_name: str = None,
+    ):
+        """Process a single block in the CF overrides or CF supplements region
+        of the configuration file. First check that the applicability
+        matches the mission and short name for the class. Next, check
+        for a variable pattern. This is indicative of there being
+        overriding or supplemental attributes in this list item.
+        Assign any information to the results dictionary, with a key of
+        that variable pattern. Lastly, check for any nested references,
+        which are child blocks to be processed in the same way. The mission
+        and short name from this block are passed to all children, as they
+        may not both be defined, due to assumed inheritance.
 
         """
         mission = cf_item['Applicability'].get('Mission') or input_mission
         short_name = cf_item['Applicability'].get('ShortNamePath') or input_short_name
 
         if mission is not None and self._is_applicable(mission, short_name):
             # Some outer Applicability items have attributes, but no
@@ -160,52 +175,54 @@
 
             if 'Attributes' in cf_item:
                 results[pattern] = self._create_attributes_object(cf_item)
 
             cf_references = cf_item.get('Applicability_Group', [])
 
             for cf_reference in cf_references:
-                self._process_cf_item(cf_reference, results, mission,
-                                      short_name)
+                self._process_cf_item(cf_reference, results, mission, short_name)
 
     @staticmethod
     def _create_attributes_object(cf_item: Dict) -> Dict[str, str]:
-        """ Construct a dictionary object containing all contained attributes,
-            which are specified as list items with Name and Value keys.
+        """Construct a dictionary object containing all contained attributes,
+        which are specified as list items with Name and Value keys.
 
         """
-        return {attribute['Name']: attribute['Value']
-                for attribute in cf_item.get('Attributes', {})}
+        return {
+            attribute['Name']: attribute['Value']
+            for attribute in cf_item.get('Attributes', {})
+        }
 
     def get_cf_attributes(self, variable: str = None) -> Dict[str, Dict[str, str]]:
-        """ Return the CF overrides and supplements that match a given
-            variable. If a variable is not specified, then return all overrides
-            and supplements. If there are no overrides or supplements, then
-            empty dictionaries will be returned instead.
+        """Return the CF overrides and supplements that match a given
+        variable. If a variable is not specified, then return all overrides
+        and supplements. If there are no overrides or supplements, then
+        empty dictionaries will be returned instead.
 
         """
         if variable is not None:
-            cf_overrides = self._get_matching_attributes(self._cf_overrides,
-                                                         variable)
-            cf_supplements = self._get_matching_attributes(self._cf_supplements,
-                                                           variable)
+            cf_overrides = self._get_matching_attributes(self._cf_overrides, variable)
+            cf_supplements = self._get_matching_attributes(
+                self._cf_supplements, variable
+            )
         else:
             cf_overrides = self._cf_overrides
             cf_supplements = self._cf_supplements
 
         return {'cf_overrides': cf_overrides, 'cf_supplements': cf_supplements}
 
     @staticmethod
-    def _get_matching_attributes(cf_references: Dict[str, Dict[str, str]],
-                                 variable: str) -> Dict[str, str]:
-        """ Iterate through either the self._cf_supplements or
-            self._cf_overrides and extract a dictionary that combines all
-            applicable attributes that apply to the specified variable. If
-            there are conflicting values for the same attribute, only the last
-            value will be returned for that attribute.
+    def _get_matching_attributes(
+        cf_references: Dict[str, Dict[str, str]], variable: str
+    ) -> Dict[str, str]:
+        """Iterate through either the self._cf_supplements or
+        self._cf_overrides and extract a dictionary that combines all
+        applicable attributes that apply to the specified variable. If
+        there are conflicting values for the same attribute, only the last
+        value will be returned for that attribute.
 
         """
         references = {}
         for pattern, attributes in cf_references.items():
             if re.match(pattern, variable) is not None:
                 references.update(attributes)
```

### Comparing `earthdata-varinfo-2.2.0/varinfo/cmr_search.py` & `earthdata-varinfo-2.2.1/varinfo/cmr_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,179 +1,189 @@
-''' This script leverages the `python-cmr` library to conduct a CMR search
+""" This script leverages the `python-cmr` library to conduct a CMR search
     and get a granule download URL. With the granule download URL and the
     `requests` library a granule is downloaded via https and saved locally.
-'''
+"""
 
 from typing import Literal, Union
 import os.path
 
 from cmr import GranuleQuery, CMR_OPS, CMR_SIT, CMR_UAT
 import requests
 
-from varinfo.exceptions import (CMRQueryException,
-                                MissingGranuleDownloadLinks,
-                                MissingPositionalArguments,
-                                GranuleDownloadException,
-                                DirectoryCreationException,
-                                GetEdlTokenException)
+from varinfo.exceptions import (
+    CMRQueryException,
+    MissingGranuleDownloadLinks,
+    MissingPositionalArguments,
+    GranuleDownloadException,
+    DirectoryCreationException,
+    GetEdlTokenException,
+)
 
 
 CmrEnvType = Literal[CMR_OPS, CMR_UAT, CMR_SIT]
 urs_token_endpoints = {
     CMR_OPS: 'https://urs.earthdata.nasa.gov/api/nams/edl_user_token',
     CMR_UAT: 'https://uat.urs.earthdata.nasa.gov/api/nams/edl_user_token',
-    CMR_SIT: 'https://sit.urs.earthdata.nasa.gov/api/nams/edl_user_token'}
+    CMR_SIT: 'https://sit.urs.earthdata.nasa.gov/api/nams/edl_user_token',
+}
 
 
-def get_granules(concept_id: str = None,
-                 collection_shortname: str = None,
-                 collection_version: str = None,
-                 provider: str = None,
-                 cmr_env: CmrEnvType = CMR_OPS,
-                 auth_header: str = None) -> list:
-    ''' Search CMR to retrieve granules for a specific collection given:
-
-        * concept_id: a CMR collection or granule concept ID. For most
-          workflows, including the generateVariableDrafts within the CMR
-          GraphQL interface, this is anticipated to be a collection concept ID,
-          but the `GranuleQuery` object can also make queries with a granule
-          concept IDs.
-        * shortname/short_name: e.g., 'SNDRSNIML2CCPRET' or 'M2T1NXSLV'
-        * collection_version/version: a collection version: '2' or 5.12.4'
-        * provider: data center ID (e.g. GES_DISC, PODAAC, POCLOUD, EEDTEST)
-        * cmr_env/mode: CMR environments (OPS, UAT, and SIT)
-        * auth_header: Authorization HTTP header, either:
-          - A header with a LaunchPad token: 'Authorization: <token>'
-          - A header with an EDL bearer token: 'Authorization: Bearer <token>'
+def get_granules(
+    concept_id: str = None,
+    collection_shortname: str = None,
+    collection_version: str = None,
+    provider: str = None,
+    cmr_env: CmrEnvType = CMR_OPS,
+    auth_header: str = None,
+) -> list:
+    """Search CMR to retrieve granules for a specific collection given:
+
+    * concept_id: a CMR collection or granule concept ID. For most
+      workflows, including the generateVariableDrafts within the CMR
+      GraphQL interface, this is anticipated to be a collection concept ID,
+      but the `GranuleQuery` object can also make queries with a granule
+      concept IDs.
+    * shortname/short_name: e.g., 'SNDRSNIML2CCPRET' or 'M2T1NXSLV'
+    * collection_version/version: a collection version: '2' or 5.12.4'
+    * provider: data center ID (e.g. GES_DISC, PODAAC, POCLOUD, EEDTEST)
+    * cmr_env/mode: CMR environments (OPS, UAT, and SIT)
+    * auth_header: Authorization HTTP header, either:
+      - A header with a LaunchPad token: 'Authorization: <token>'
+      - A header with an EDL bearer token: 'Authorization: Bearer <token>'
 
-        For a successful search response concept_id or short_name, version and
-        provider must be entered along with a bearer_token.
+    For a successful search response concept_id or short_name, version and
+    provider must be entered along with a bearer_token.
 
-    '''
+    """
     granule_query = GranuleQuery(mode=cmr_env)
 
     # Ensure the Authorization header was provided for CMR authentication
     if auth_header is not None:
         granule_query.headers = {'Authorization': auth_header}
     else:
         raise MissingPositionalArguments('auth_header')
 
     if concept_id is not None:
         # If a collection or granule concept ID is specified, can query CMR
         # just using that parameter.
         query_parameters = {'concept_id': concept_id}
     elif collection_shortname and collection_version and provider is not None:
         # Otherwise use the combination of short_name, version, and provider
-        query_parameters = {'short_name': collection_shortname,
-                            'version': collection_version,
-                            'provider': provider}
+        query_parameters = {
+            'short_name': collection_shortname,
+            'version': collection_version,
+            'provider': provider,
+        }
     else:
         # If neither condition is met, there aren't enough CMR query parameters
         # to identify the collection.
-        raise MissingPositionalArguments('concept_id or collection_shortname, '
-                                         'collection_version, and provider')
+        raise MissingPositionalArguments(
+            'concept_id or collection_shortname, ' 'collection_version, and provider'
+        )
 
     # Assign parameters to GranuleQuery
-    granule_query.parameters(downloadable=True,
-                             sort_key='-start_date',
-                             **query_parameters)
+    granule_query.parameters(
+        downloadable=True, sort_key='-start_date', **query_parameters
+    )
     try:
         # .get() is the number of links to return (e.g. page_size)
         granule_response = granule_query.get(10)
 
     except Exception as cmr_exception:
         # Capture exception raised due to CMR failure and return an exception
         # with a more user-friendly message.
         raise CMRQueryException(str(cmr_exception)) from cmr_exception
 
     if len(granule_response) == 0:
         # No granules were identified, so no files can be downloaded and parsed
-        raise IndexError('No granules were found with selected '
-                         'parameters and user permissions')
+        raise IndexError(
+            'No granules were found with selected ' 'parameters and user permissions'
+        )
 
     return granule_response
 
 
 def get_granule_link(granule_response: list) -> str:
-    ''' Get the granule download link from CMR. '''
-    granule_link = next((link['href']
-                         for link in granule_response[0].get('links', [])
-                         if link['rel'].endswith('/data#') and 'inherited' not in link), None)
+    """Get the granule download link from CMR."""
+    granule_link = next(
+        (
+            link['href']
+            for link in granule_response[0].get('links', [])
+            if link['rel'].endswith('/data#') and 'inherited' not in link
+        ),
+        None,
+    )
 
     if granule_link is None:
         raise MissingGranuleDownloadLinks(granule_response)
 
     return granule_link
 
 
-def download_granule(granule_link: str,
-                     auth_header: str,
-                     out_directory: str = os.getcwd()) -> str:
-    ''' Use the requests module to download data via https.
-        * granule_link: granule download URL.
-        * auth_header: Authorization HTTP header, either:
-          - A header with a LaunchPad token: 'Authorization: <token>'
-          - A header with an EDL bearer token: 'Authorization: Bearer <token>'
-        * out_directory: path to save downloaded granule
-            (the default is the current directory).
-    '''
+def download_granule(
+    granule_link: str, auth_header: str, out_directory: str = os.getcwd()
+) -> str:
+    """Use the requests module to download data via https.
+    * granule_link: granule download URL.
+    * auth_header: Authorization HTTP header, either:
+      - A header with a LaunchPad token: 'Authorization: <token>'
+      - A header with an EDL bearer token: 'Authorization: Bearer <token>'
+    * out_directory: path to save downloaded granule
+        (the default is the current directory).
+    """
     # Create `out_directory` if it does not exist and create out_filename
     if not os.path.isdir(out_directory):
         try:
             os.mkdir(out_directory)
         except Exception as os_exception:
-            raise DirectoryCreationException(
-                str(os_exception)) from os_exception
+            raise DirectoryCreationException(str(os_exception)) from os_exception
 
     out_filename = os.path.join(out_directory, os.path.basename(granule_link))
 
     try:
         # Write content of data to out_filename and return response
-        response = requests.get(granule_link,
-                                headers={'Authorization': auth_header},
-                                timeout=10)
+        response = requests.get(
+            granule_link, headers={'Authorization': auth_header}, timeout=10
+        )
 
         with open(out_filename, 'wb') as file_download:
             file_download.write(response.content)
 
         return out_filename
     except Exception as requests_exception:
         # Custom exception for error from `requests.get`
-        raise GranuleDownloadException(
-            str(requests_exception)) from requests_exception
+        raise GranuleDownloadException(str(requests_exception)) from requests_exception
 
 
-def get_edl_token_from_launchpad(launchpad_token: str,
-                                 cmr_env: CmrEnvType) -> Union[str, None]:
-    ''' Retrieve an EDL token given a LaunchPad token.
-        * launchpad_token: A LaunchPad token with no header prefixes:
-          <Launchpad token>
-        * cmr_env/mode: CMR environments (OPS, UAT, and SIT)
-    '''
+def get_edl_token_from_launchpad(
+    launchpad_token: str, cmr_env: CmrEnvType
+) -> Union[str, None]:
+    """Retrieve an EDL token given a LaunchPad token.
+    * launchpad_token: A LaunchPad token with no header prefixes:
+      <Launchpad token>
+    * cmr_env/mode: CMR environments (OPS, UAT, and SIT)
+    """
     url_urs_endpoint = urs_token_endpoints.get(cmr_env)
     try:
-        response = requests.post(url=url_urs_endpoint,
-                                 data=f'token={launchpad_token}',
-                                 timeout=10)
+        response = requests.post(
+            url=url_urs_endpoint, data=f'token={launchpad_token}', timeout=10
+        )
         response.raise_for_status()
 
     except Exception as requests_exception:
-        raise GetEdlTokenException(
-            str(requests_exception)) from requests_exception
+        raise GetEdlTokenException(str(requests_exception)) from requests_exception
 
     return response.json().get('access_token')
 
 
 def get_edl_token_header(auth_header: str, cmr_env: CmrEnvType) -> str:
-    ''' Helper function for getting the header for an EDL token.
-        * auth_header: Authorization HTTP header, either:
-          - A header with a LaunchPad token: 'Authorization: <token>'
-          - A header with an EDL bearer token: 'Authorization: Bearer <token>'
-        * cmr_env/mode: CMR environments (OPS, UAT, and SIT)
-    '''
+    """Helper function for getting the header for an EDL token.
+    * auth_header: Authorization HTTP header, either:
+      - A header with a LaunchPad token: 'Authorization: <token>'
+      - A header with an EDL bearer token: 'Authorization: Bearer <token>'
+    * cmr_env/mode: CMR environments (OPS, UAT, and SIT)
+    """
     if 'Bearer ' not in auth_header:
-        edl_auth_header = (
-            f'Bearer {get_edl_token_from_launchpad(auth_header, cmr_env)}'
-        )
+        edl_auth_header = f'Bearer {get_edl_token_from_launchpad(auth_header, cmr_env)}'
     else:
         edl_auth_header = auth_header
     return edl_auth_header
```

### Comparing `earthdata-varinfo-2.2.0/varinfo/exceptions.py` & `earthdata-varinfo-2.2.1/varinfo/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,123 +3,137 @@
     of the expected errors that may occur during an invocation of the package,
     or any third party code that uses the package.
 
 """
 
 
 class CustomError(Exception):
-    """ Base class for exceptions in `earthdata-varinfo`. This base class
-        allows for future work, such as assigning exit codes for specific
-        failure modes.
+    """Base class for exceptions in `earthdata-varinfo`. This base class
+    allows for future work, such as assigning exit codes for specific
+    failure modes.
 
     """
 
     def __init__(self, exception_type, message):
         self.exception_type = exception_type
         self.message = message
         super().__init__(self.message)
 
 
 class DmrNamespaceError(CustomError):
-    """ This exception is raised when the root element of a dmr XML document
-        is not a fully qualified Dataset tag.
+    """This exception is raised when the root element of a dmr XML document
+    is not a fully qualified Dataset tag.
 
     """
 
     def __init__(self, tag):
         super().__init__('DmrNamespaceError', f'Unexpected root: {tag}')
 
 
 class InvalidConfigFileFormatError(CustomError):
-    """ This exception is raised when a configuration file is specified when
-        creating an instance of a VarInfo or CFConfig class with a non ".json"
-        extension.
+    """This exception is raised when a configuration file is specified when
+    creating an instance of a VarInfo or CFConfig class with a non ".json"
+    extension.
 
     """
 
     def __init__(self, file_path):
-        super().__init__('InvalidConfigFileFormatError',
-                         f'"{file_path}" must be a JSON file.')
+        super().__init__(
+            'InvalidConfigFileFormatError', f'"{file_path}" must be a JSON file.'
+        )
 
 
 class InvalidExportDirectory(CustomError):
-    """ This exception is raised when an output directory is specified for
-        variable record export, and a file exists at that location instead.
+    """This exception is raised when an output directory is specified for
+    variable record export, and a file exists at that location instead.
 
     """
 
     def __init__(self, directory_path):
-        super().__init__('InvalidExportDirectory',
-                         f'"{directory_path}" cannot be an existing file.')
+        super().__init__(
+            'InvalidExportDirectory', f'"{directory_path}" cannot be an existing file.'
+        )
 
 
 class MissingConfigurationFileError(CustomError):
-    """ This exception is raised when a configuration file path is supplied to
-        either a VarInfo class or the CFConfig class, but there is no file at
-        the specified location.
+    """This exception is raised when a configuration file path is supplied to
+    either a VarInfo class or the CFConfig class, but there is no file at
+    the specified location.
 
     """
 
     def __init__(self, file_path):
-        super().__init__('MissingConfigurationFileError',
-                         f'No file in specified location: {file_path}')
+        super().__init__(
+            'MissingConfigurationFileError',
+            f'No file in specified location: {file_path}',
+        )
 
 
 class CMRQueryException(CustomError):
-    ''' This exception is raised when a query to CMR fails.
-    '''
+    """This exception is raised when a query to CMR fails."""
 
     def __init__(self, cmr_exception_message):
-        super().__init__('CMRQueryException',
-                         'CMR query failed with the following error: '
-                         f'{cmr_exception_message}')
+        super().__init__(
+            'CMRQueryException',
+            'CMR query failed with the following error: ' f'{cmr_exception_message}',
+        )
 
 
 class MissingPositionalArguments(CustomError):
-    ''' This exception is raised when a function is missing a required
-        positional argument.
-    '''
+    """This exception is raised when a function is missing a required
+    positional argument.
+    """
 
     def __init__(self, positional_argument):
-        super().__init__('MissingPositionalArguments',
-                         f'Missing positional argument: {positional_argument}')
+        super().__init__(
+            'MissingPositionalArguments',
+            f'Missing positional argument: {positional_argument}',
+        )
 
 
 class MissingGranuleDownloadLinks(CustomError):
-    ''' This exception is raised when a granule record does not contain links
-        to download data.
-    '''
+    """This exception is raised when a granule record does not contain links
+    to download data.
+    """
 
     def __init__(self, download_link):
-        super().__init__('MissingGranuleDownloadLinks',
-                         f'No links for granule record: {download_link}')
+        super().__init__(
+            'MissingGranuleDownloadLinks',
+            f'No links for granule record: {download_link}',
+        )
 
 
 class GranuleDownloadException(CustomError):
-    ''' This exception is raised when the `requests.get` modules fails
-        to download a variable locally.
-    '''
+    """This exception is raised when the `requests.get` modules fails
+    to download a variable locally.
+    """
 
     def __init__(self, granule_download_exception_message):
-        super().__init__('GranuleDownloadException',
-                         'requests module failed with the following error: '
-                         f'{granule_download_exception_message}')
+        super().__init__(
+            'GranuleDownloadException',
+            'requests module failed with the following error: '
+            f'{granule_download_exception_message}',
+        )
 
 
 class DirectoryCreationException(CustomError):
-    ''' This exception is raised when creating a directory fails.
-    '''
+    """This exception is raised when creating a directory fails."""
 
     def __init__(self, directory_creation_exception_message):
-        super().__init__('DirectoryCreationException',
-                         'directory creation failed with the following error: '
-                         f'{directory_creation_exception_message}')
+        super().__init__(
+            'DirectoryCreationException',
+            'directory creation failed with the following error: '
+            f'{directory_creation_exception_message}',
+        )
 
 
 class GetEdlTokenException(CustomError):
-    ''' This exception is raised when `requests.post` fails to get an
-        EDL token given a LaunchPad token
-    '''
+    """This exception is raised when `requests.post` fails to get an
+    EDL token given a LaunchPad token
+    """
+
     def __init__(self, get_edl_token_exception_message):
-        super().__init__('GetEdlTokenException',
-                         'requests module failed with the following error: '
-                         f'{get_edl_token_exception_message}')
+        super().__init__(
+            'GetEdlTokenException',
+            'requests module failed with the following error: '
+            f'{get_edl_token_exception_message}',
+        )
```

### Comparing `earthdata-varinfo-2.2.0/varinfo/generate_umm_var.py` & `earthdata-varinfo-2.2.1/varinfo/generate_umm_var.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,111 @@
-''' This module generates UMM-Var records for a specified collection, and
+""" This module generates UMM-Var records for a specified collection, and
     optionally will publish those records to CMR.
     `generation_collection_umm_var` will:
 
     * Performing a CMR granule search with collection-based query parameters.
     * Downloading the granule locally.
     * Parse the variable metadata from the granule using VarInfoFromNetCDF4.
     * Generate UMM-Var JSON as a dictionary for each identified variable.
     * (Optional) Publish each UMM-Var entry to the selected CMR environment.
 
-'''
+"""
+
 from tempfile import TemporaryDirectory
 from typing import Dict, List, Union
 import re
 
 from cmr import CMR_UAT
 
 from varinfo import VarInfoFromNetCDF4
-from varinfo.cmr_search import (CmrEnvType, download_granule, get_granule_link,
-                                get_granules, get_edl_token_header)
+from varinfo.cmr_search import (
+    CmrEnvType,
+    download_granule,
+    get_granule_link,
+    get_granules,
+    get_edl_token_header,
+)
 from varinfo.umm_var import get_all_umm_var, publish_all_umm_var
 
 
 # Custom return type: either a list of UMM-Var JSON (a list of dictionaries),
 # or a list of strings (either concept IDs or error strings).
 UmmVarReturnType = List[Union[Dict, str]]
 
 
-def generate_collection_umm_var(collection_concept_id: str,
-                                auth_header: str,
-                                cmr_env: CmrEnvType = CMR_UAT,
-                                publish: bool = False) -> UmmVarReturnType:
-    """ Run all the of the functions for downloading and publishing
-        a UMM-Var entry to CMR given:
-
-        * collection_concept_id: Concept ID for collection that variables have
-          been generated for.
-        * cmr_env: URLs for CMR environments (OPS, UAT, and SIT)
-        * auth_header: Authorization HTTP header, containing a LaunchPad
-          token: 'Authorization: <token>'
-        * publish: Optional argument determining whether to publish the
-          generated UMM-Var records to the indicated CMR instance. Defaults to
-          False.
+def generate_collection_umm_var(
+    collection_concept_id: str,
+    auth_header: str,
+    cmr_env: CmrEnvType = CMR_UAT,
+    publish: bool = False,
+) -> UmmVarReturnType:
+    """Run all the of the functions for downloading and publishing
+    a UMM-Var entry to CMR given:
+
+    * collection_concept_id: Concept ID for collection that variables have
+      been generated for.
+    * cmr_env: URLs for CMR environments (OPS, UAT, and SIT)
+    * auth_header: Authorization HTTP header, containing a LaunchPad
+      token: 'Authorization: <token>'
+    * publish: Optional argument determining whether to publish the
+      generated UMM-Var records to the indicated CMR instance. Defaults to
+      False.
 
-        Note - if attempting to publish to CMR, a LaunchPad token must be used.
+    Note - if attempting to publish to CMR, a LaunchPad token must be used.
 
     """
     # Get an EDL token and its header given a LaunchPad token
     auth_header_edl_token = get_edl_token_header(auth_header, cmr_env)
 
-    granule_response = get_granules(collection_concept_id, cmr_env=cmr_env,
-                                    auth_header=auth_header_edl_token)
+    granule_response = get_granules(
+        collection_concept_id, cmr_env=cmr_env, auth_header=auth_header_edl_token
+    )
 
     # Get the data download URL for the most recent granule (NetCDF-4 file)
     granule_link = get_granule_link(granule_response)
 
     with TemporaryDirectory() as temp_dir:
         # Download file to runtime environment
-        local_granule = download_granule(granule_link,
-                                         auth_header_edl_token,
-                                         out_directory=temp_dir)
+        local_granule = download_granule(
+            granule_link, auth_header_edl_token, out_directory=temp_dir
+        )
 
         # Parse the granule with VarInfo to map all variables and relations:
         var_info = VarInfoFromNetCDF4(local_granule)
 
         # Generate all the UMM-Var records:
         all_umm_var_records = get_all_umm_var(var_info)
 
     if publish:
         # Publish to CMR and construct an output object that is a list of
         # strings. These strings will be either variable concept IDs or
         # error messages returned from CMR.
-        publication_response = publish_all_umm_var(collection_concept_id,
-                                                   all_umm_var_records,
-                                                   auth_header, cmr_env)
+        publication_response = publish_all_umm_var(
+            collection_concept_id, all_umm_var_records, auth_header, cmr_env
+        )
 
         # Produce a list indicating publication information for all variables.
         # Variables that were successfully published will have a list element
         # providing their variable concept ID. Any variables that were
         # not successfully published will instead have an element containing
         # the variable name and the CMR error (e.g., 'variable: CMR error...').
-        return_value = [variable_response
-                        if is_variable_concept_id(variable_response)
-                        else ': '.join([variable_name, variable_response])
-                        for variable_name, variable_response
-                        in publication_response.items()]
+        return_value = [
+            (
+                variable_response
+                if is_variable_concept_id(variable_response)
+                else ': '.join([variable_name, variable_response])
+            )
+            for variable_name, variable_response in publication_response.items()
+        ]
     else:
         # If not publishing, return the full UMM-Var JSON records
         return_value = list(all_umm_var_records.values())
 
     return return_value
 
 
 def is_variable_concept_id(possible_concept_id: str) -> bool:
-    """ A helper function to identify if a given string conforms to the
-        expected structure of a variable concept ID, e.g., 'V1234567890-PROV'.
+    """A helper function to identify if a given string conforms to the
+    expected structure of a variable concept ID, e.g., 'V1234567890-PROV'.
 
     """
     return bool(re.match(r'^V\d{10}-\w+$', possible_concept_id))
```

### Comparing `earthdata-varinfo-2.2.0/varinfo/umm_var.py` & `earthdata-varinfo-2.2.1/varinfo/umm_var.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         umm_var_schema = json.load(file_handler)
 
     for record in umm_var_records:
         validate(schema=umm_var_schema, instance=umm_var_schema)
     ```
 
 """
+
 from os import makedirs
 from os.path import isfile, join as join_path
 from typing import Any, Dict, List, Optional, Union
 import json
 import requests
 
 from cmr import CMR_UAT
@@ -44,159 +45,191 @@
 from varinfo.var_info import VarInfoBase
 from varinfo.variable import VariableBase
 
 
 UMM_URL = 'https://cdn.earthdata.nasa.gov/umm'
 UMM_VAR_VERSION = '1.8.2'
 
-UMM_VAR_DTYPES = ['byte', 'float', 'float32', 'float64', 'double', 'ubyte',
-                  'ushort', 'uint', 'uchar', 'string', 'char8', 'uchar8',
-                  'short', 'long', 'int', 'int8', 'int16', 'int32', 'int64',
-                  'uint8', 'uint16', 'uint32', 'uint64', 'OTHER']
+UMM_VAR_DTYPES = [
+    'byte',
+    'float',
+    'float32',
+    'float64',
+    'double',
+    'ubyte',
+    'ushort',
+    'uint',
+    'uchar',
+    'string',
+    'char8',
+    'uchar8',
+    'short',
+    'long',
+    'int',
+    'int8',
+    'int16',
+    'int32',
+    'int64',
+    'uint8',
+    'uint16',
+    'uint32',
+    'uint64',
+    'OTHER',
+]
 
 
 def get_all_umm_var(var_info: VarInfoBase) -> Dict[str, Dict]:
-    """ Iterate through all variables detected from the source granule and
-        return a list of UMM-Var records for those variables.
+    """Iterate through all variables detected from the source granule and
+    return a list of UMM-Var records for those variables.
 
     """
-    return {variable_name: get_umm_var(var_info, variable)
-            for variable_name, variable in var_info.variables.items()}
+    return {
+        variable_name: get_umm_var(var_info, variable)
+        for variable_name, variable in var_info.variables.items()
+    }
 
 
 def get_umm_var(var_info: VarInfoBase, variable: VariableBase) -> Dict:
-    """ Map the contents of a Variable instance to a UMM-Var record.
-        Initial attempts will be made to extract all possibly information,
-        with the return value being scrubbed of all UMM-Var attributes with
-        None values.
+    """Map the contents of a Variable instance to a UMM-Var record.
+    Initial attempts will be made to extract all possibly information,
+    with the return value being scrubbed of all UMM-Var attributes with
+    None values.
 
     """
     variable_name = variable.full_name_path.lstrip('/')
     umm_var_record = {
         'Name': variable_name,
-        'LongName': get_first_matched_attribute(variable, ['long_name'],
-                                                variable_name),
-        'StandardName': get_first_matched_attribute(variable,
-                                                    ['standard_name']),
+        'LongName': get_first_matched_attribute(variable, ['long_name'], variable_name),
+        'StandardName': get_first_matched_attribute(variable, ['standard_name']),
         'Definition': get_first_matched_attribute(
             variable,
-            ['description', 'Description', 'definition', 'Definition',
-             'title', 'Title'],
-            variable_name
+            [
+                'description',
+                'Description',
+                'definition',
+                'Definition',
+                'title',
+                'Title',
+            ],
+            variable_name,
         ),
         'DataType': get_umm_var_dtype(variable.data_type),
         'Dimensions': get_dimensions(var_info, variable),
         'Units': get_first_matched_attribute(variable, ['units', 'Units']),
         'FillValues': get_fill_values(variable),
         'Scale': get_first_matched_attribute(
             variable, ['scale_factor', 'scale', 'Scale']
         ),
         'Offset': get_first_matched_attribute(
             variable, ['add_offset', 'offset', 'Offset']
         ),
         'ValidRanges': get_valid_ranges(variable),
         'VariableType': get_variable_type(var_info, variable),
-        'MetadataSpecification': get_metadata_specification()
+        'MetadataSpecification': get_metadata_specification(),
     }
 
-    return {umm_var_attribute: umm_var_value
-            for umm_var_attribute, umm_var_value
-            in umm_var_record.items()
-            if umm_var_value is not None}
+    return {
+        umm_var_attribute: umm_var_value
+        for umm_var_attribute, umm_var_value in umm_var_record.items()
+        if umm_var_value is not None
+    }
 
 
 def export_all_umm_var_to_json(umm_var_records: List, output_dir: str = '.'):
-    """ Iterate through a list of UMM-Var JSON records and save them all to
-        files (one file per record).
+    """Iterate through a list of UMM-Var JSON records and save them all to
+    files (one file per record).
 
-        The output file name will be the full path of each variable will be the
-        full path of the variable, with any slashes replaced with underscores.
+    The output file name will be the full path of each variable will be the
+    full path of the variable, with any slashes replaced with underscores.
 
     """
     for umm_var_record in umm_var_records:
         export_umm_var_to_json(umm_var_record, output_dir)
 
 
 def export_umm_var_to_json(umm_var_record: Dict, output_dir: str = '.'):
-    """ Export a single UMM-Var JSON object to a JSON output file in a
-        specified directory (the default is the directory in which the function
-        is called). If the specified directory does not exist, it will be
-        created.
+    """Export a single UMM-Var JSON object to a JSON output file in a
+    specified directory (the default is the directory in which the function
+    is called). If the specified directory does not exist, it will be
+    created.
 
-        The output file name will be the full path of the variable, with any
-        slashes replaced with underscores.
+    The output file name will be the full path of the variable, with any
+    slashes replaced with underscores.
 
     """
     if isfile(output_dir):
         raise InvalidExportDirectory(output_dir)
     else:
         # `exists_ok=True` makes this a no-op for existing directories:
         makedirs(output_dir, exist_ok=True)
 
     output_file_path = join_path(
-        output_dir,
-        f'{umm_var_record["Name"].replace("/", "_")}.json'
+        output_dir, f'{umm_var_record["Name"].replace("/", "_")}.json'
     )
 
     with open(output_file_path, 'w', encoding='utf-8') as file_handler:
         json.dump(umm_var_record, file_handler, indent=2)
 
 
-def get_first_matched_attribute(variable: VariableBase,
-                                attribute_names: List[str],
-                                default_value: Any = None) -> Any:
-    """ Check a list of metadata attributes and return the value of the first
-        one that is present in the Variable. If none of the attributes are
-        in the variable metadata, return the supplied default value.
+def get_first_matched_attribute(
+    variable: VariableBase, attribute_names: List[str], default_value: Any = None
+) -> Any:
+    """Check a list of metadata attributes and return the value of the first
+    one that is present in the Variable. If none of the attributes are
+    in the variable metadata, return the supplied default value.
 
     """
     return next(
-        (get_json_serializable_value(variable.attributes.get(attribute_name))
-         for attribute_name in attribute_names
-         if attribute_name in variable.attributes),
-        default_value
+        (
+            get_json_serializable_value(variable.attributes.get(attribute_name))
+            for attribute_name in attribute_names
+            if attribute_name in variable.attributes
+        ),
+        default_value,
     )
 
 
-def get_dimensions(var_info: VarInfoBase,
-                   variable: VariableBase) -> Optional[List]:
-    """ Return a list of all dimensions for the variable, """
-    dimensions = [get_dimension_information(var_info, variable, dimension_name)
-                  for dimension_name in variable.dimensions]
+def get_dimensions(var_info: VarInfoBase, variable: VariableBase) -> Optional[List]:
+    """Return a list of all dimensions for the variable,"""
+    dimensions = [
+        get_dimension_information(var_info, variable, dimension_name)
+        for dimension_name in variable.dimensions
+    ]
 
     if len(dimensions) == 0:
         dimensions = None
 
     return dimensions
 
 
-def get_dimension_information(var_info: VarInfoBase, variable: VariableBase,
-                              dimension_name: str) -> Dict:
-    """ Retrieve a DimensionType object for the given Variable dimension. This
-        function is only called for named dimensions listed in the `dimensions`
-        attribute of another variable, and so should exist as at least a
-        dimension within the source file.
-
-        The dimension types in earthdata-varinfo are currently limited to
-        horizontal spatial dimensions (e.g., lat, lon, projected x or projected
-        y), or temporal dimensions based on the available heuristics in the
-        VariableBase class.
-
-        The dimension Name property is the full path to the variable, omitting
-        any leading slashes. (E.g., a variable located at "/group/variable"
-        within a file will extract a name of "group/variable")
-
-        Currently unsupported dimension types (will have type: 'OTHER'):
-
-        * Vertical dimensions (pressure, height, depth).
-        * Projected horizontal spatial dimension (no UMM-Var type for this).
-        * Swath dimensions (along or across track).
+def get_dimension_information(
+    var_info: VarInfoBase, variable: VariableBase, dimension_name: str
+) -> Dict:
+    """Retrieve a DimensionType object for the given Variable dimension. This
+    function is only called for named dimensions listed in the `dimensions`
+    attribute of another variable, and so should exist as at least a
+    dimension within the source file.
+
+    The dimension types in earthdata-varinfo are currently limited to
+    horizontal spatial dimensions (e.g., lat, lon, projected x or projected
+    y), or temporal dimensions based on the available heuristics in the
+    VariableBase class.
+
+    The dimension Name property is the full path to the variable, omitting
+    any leading slashes. (E.g., a variable located at "/group/variable"
+    within a file will extract a name of "group/variable")
+
+    Currently unsupported dimension types (will have type: 'OTHER'):
+
+    * Vertical dimensions (pressure, height, depth).
+    * Projected horizontal spatial dimension (no UMM-Var type for this).
+    * Swath dimensions (along or across track).
 
-        Also note: VariableFromDmr instances do not currently extract variable
-        shapes.
+    Also note: VariableFromDmr instances do not currently extract variable
+    shapes.
 
     """
     dimension_variable = var_info.get_variable(dimension_name)
 
     if dimension_variable is not None:
         dimension_name = dimension_variable.full_name_path
         if dimension_variable.is_latitude():
@@ -209,35 +242,38 @@
             dimension_type = 'OTHER'
 
     else:
         # Dimension without variable, potentially used only to denote array
         # size in a specific, non-physical dimension (e.g., nv, latv, lonv).
         dimension_type = 'OTHER'
 
-    return {'Name': dimension_name.lstrip('/'),
-            'Size': get_dimension_size(var_info, variable, dimension_name),
-            'Type': dimension_type}
-
-
-def get_dimension_size(var_info: VarInfoBase, variable_with_dim: VariableBase,
-                       dimension_name: str) -> Union[str, int]:
-    """ Extract the size of a specific dimension for a variable. This
-        function will attempt to retrieve the dimension size from the following
-        locations (in the order given):
-
-        * The shape of the variable with the dimension itself, if present.
-        * The shape of the 1-D dimension variable corresponding to the
-          dimension for which the size is requested.
-        * The variable will be checked for known names, as described in the
-          CF-Conventions, to assign a length (relating to bounds variables).
-        * If no other condition is met, the size of 'Varies' is returned.
-
-        Note, this function is only called via an iteration through the
-        `variable_with_dim.dimensions` list, and so `dimension_name` should
-        always be present in that list.
+    return {
+        'Name': dimension_name.lstrip('/'),
+        'Size': get_dimension_size(var_info, variable, dimension_name),
+        'Type': dimension_type,
+    }
+
+
+def get_dimension_size(
+    var_info: VarInfoBase, variable_with_dim: VariableBase, dimension_name: str
+) -> Union[str, int]:
+    """Extract the size of a specific dimension for a variable. This
+    function will attempt to retrieve the dimension size from the following
+    locations (in the order given):
+
+    * The shape of the variable with the dimension itself, if present.
+    * The shape of the 1-D dimension variable corresponding to the
+      dimension for which the size is requested.
+    * The variable will be checked for known names, as described in the
+      CF-Conventions, to assign a length (relating to bounds variables).
+    * If no other condition is met, the size of 'Varies' is returned.
+
+    Note, this function is only called via an iteration through the
+    `variable_with_dim.dimensions` list, and so `dimension_name` should
+    always be present in that list.
 
     """
     dimension_variable = var_info.get_variable(dimension_name)
 
     if variable_with_dim.shape is not None:
         dimension_index = variable_with_dim.dimensions.index(dimension_name)
         dimension_size = variable_with_dim.shape[dimension_index]
@@ -261,172 +297,184 @@
         # array size in a specific, non-physical dimension
         dimension_size = 'Varies'
 
     return dimension_size
 
 
 def get_valid_ranges(variable: VariableBase) -> Optional[List[Dict]]:
-    """ Return a dictionary containing the valid minimum and/or valid maximum
-        values from the variable metadata. If valid_min, valid_max or
-        valid_range are not set, None is returned.
+    """Return a dictionary containing the valid minimum and/or valid maximum
+    values from the variable metadata. If valid_min, valid_max or
+    valid_range are not set, None is returned.
 
     """
     valid_range = {
         'Min': get_json_serializable_value(variable.get_valid_min()),
-        'Max': get_json_serializable_value(variable.get_valid_max())
+        'Max': get_json_serializable_value(variable.get_valid_max()),
     }
 
     # Remove keys with None values:
-    valid_range = {range_key: range_value
-                   for range_key, range_value in valid_range.items()
-                   if range_value is not None}
+    valid_range = {
+        range_key: range_value
+        for range_key, range_value in valid_range.items()
+        if range_value is not None
+    }
 
     if len(list(valid_range.keys())) > 0:
         valid_range = [valid_range]
     else:
         valid_range = None
 
     return valid_range
 
 
 def get_fill_values(variable: VariableBase) -> Optional[List]:
-    """ Return a List containing elements of the UMM-Var FillValueType, if
-        there is a fill value contained in the variable metadata. Otherwise
-        return None.
+    """Return a List containing elements of the UMM-Var FillValueType, if
+    there is a fill value contained in the variable metadata. Otherwise
+    return None.
 
-        An initial simplification is that all fill values are of type
-        `SCIENCE_FILLVALUE`.
+    An initial simplification is that all fill values are of type
+    `SCIENCE_FILLVALUE`.
 
     """
     fill_value = get_first_matched_attribute(variable, ['_FillValue'])
     if fill_value is not None:
-        fill_values = [{
-            'Value': get_json_serializable_value(fill_value),
-            'Type': 'SCIENCE_FILLVALUE',
-            'Description': 'Extracted from _FillValue metadata attribute'
-        }]
+        fill_values = [
+            {
+                'Value': get_json_serializable_value(fill_value),
+                'Type': 'SCIENCE_FILLVALUE',
+                'Description': 'Extracted from _FillValue metadata attribute',
+            }
+        ]
     else:
         fill_values = None
 
     return fill_values
 
 
 def get_umm_var_dtype(variable_data_type: str) -> str:
-    """ Map the variable data type to a string in the UMM-Var DataTypeEnum. """
+    """Map the variable data type to a string in the UMM-Var DataTypeEnum."""
     if variable_data_type in UMM_VAR_DTYPES:
         umm_var_type = variable_data_type
     else:
         umm_var_type = 'OTHER'
 
     return umm_var_type
 
 
 def get_metadata_specification() -> Dict:
-    """ Return standard object for the UMM-Var specification, including the
-        URL, Name and Version.
+    """Return standard object for the UMM-Var specification, including the
+    URL, Name and Version.
 
     """
-    return {'URL': f'{UMM_URL}/variable/v{UMM_VAR_VERSION}',
-            'Name': 'UMM-Var',
-            'Version': UMM_VAR_VERSION}
+    return {
+        'URL': f'{UMM_URL}/variable/v{UMM_VAR_VERSION}',
+        'Name': 'UMM-Var',
+        'Version': UMM_VAR_VERSION,
+    }
 
 
 def get_json_serializable_value(input_value: Any) -> Any:
-    """ Ensure the value is JSON serializable, as some numpy float and integer
-        types are not.
+    """Ensure the value is JSON serializable, as some numpy float and integer
+    types are not.
 
     """
     if isinstance(input_value, np_integer):
         output_value = int(input_value)
     elif isinstance(input_value, np_floating):
         output_value = float(input_value)
     else:
         output_value = input_value
 
     return output_value
 
 
-def generate_variable_native_id(collection_concept_id: str,
-                                umm_var_record: Dict) -> str:
-    """ A helper function to create a CMR native ID given the collection
-        concept ID and the variable UMM-Var JSON. This native ID must be unique
-        within the entire provider. The initial implementation will be to
-        concatenate the collection concept ID and the name of the variable
-        while removing slashes that CMR will interpret as part of the URL path.
+def generate_variable_native_id(
+    collection_concept_id: str, umm_var_record: Dict
+) -> str:
+    """A helper function to create a CMR native ID given the collection
+    concept ID and the variable UMM-Var JSON. This native ID must be unique
+    within the entire provider. The initial implementation will be to
+    concatenate the collection concept ID and the name of the variable
+    while removing slashes that CMR will interpret as part of the URL path.
 
-        Note - the `Name` attribute of the generated UMM-Var record is the full
-        path of the variable.
+    Note - the `Name` attribute of the generated UMM-Var record is the full
+    path of the variable.
 
     """
-    return '-'.join([collection_concept_id,
-                     umm_var_record['Name'].replace('/', '_').lstrip('_')])
+    return '-'.join(
+        [collection_concept_id, umm_var_record['Name'].replace('/', '_').lstrip('_')]
+    )
 
 
 def get_variable_type(var_info: VarInfoBase, variable: VariableBase) -> str:
-    """ Check if a variable is a science variable and
-        map it to a 'SCIENCE_VARIABLE' if it is.
+    """Check if a variable is a science variable and
+    map it to a 'SCIENCE_VARIABLE' if it is.
     """
     if var_info.is_science_variable(variable):
         variable_type = 'SCIENCE_VARIABLE'
     else:
         variable_type = None
 
     return variable_type
 
 
-def publish_umm_var(collection_id: str,
-                    umm_var_dict: Dict,
-                    auth_header: str,
-                    cmr_env: CmrEnvType = CMR_UAT) -> str:
-    """" Publish a single UMM-Var entry to CMR given:
-        * collection_id: a collection's concept_id
-        * umm_var_dict: a dictionary of a single UMM-Var entry for a collection
-        * auth_header: Authorization HTTP header, containing a LaunchPad
-          token: 'Authorization: <token>'
-        * cmr_env: CMR environments (OPS, UAT, and SIT) default is CMR_UAT
+def publish_umm_var(
+    collection_id: str,
+    umm_var_dict: Dict,
+    auth_header: str,
+    cmr_env: CmrEnvType = CMR_UAT,
+) -> str:
+    """ " Publish a single UMM-Var entry to CMR given:
+    * collection_id: a collection's concept_id
+    * umm_var_dict: a dictionary of a single UMM-Var entry for a collection
+    * auth_header: Authorization HTTP header, containing a LaunchPad
+      token: 'Authorization: <token>'
+    * cmr_env: CMR environments (OPS, UAT, and SIT) default is CMR_UAT
 
-        For a successful requests all of these fields must be entered
+    For a successful requests all of these fields must be entered
 
     """
     # Required UMM-Var headers for ingesting variable entries
     headers_umm_var = {
         'Content-type': 'application/vnd.nasa.cmr.umm+json;version='
         + f'{umm_var_dict["MetadataSpecification"]["Version"]}',
         'Authorization': auth_header,
-        'Accept': 'application/json'
+        'Accept': 'application/json',
     }
-    variable_native_id = generate_variable_native_id(collection_id,
-                                                     umm_var_dict)
+    variable_native_id = generate_variable_native_id(collection_id, umm_var_dict)
 
-    url_endpoint = (cmr_env.replace('search', 'ingest') + 'collections/'
-                    f'{collection_id}/variables/{variable_native_id}')
+    url_endpoint = (
+        cmr_env.replace('search', 'ingest') + 'collections/'
+        f'{collection_id}/variables/{variable_native_id}'
+    )
 
-    response = requests.put(url_endpoint,
-                            json=umm_var_dict,
-                            headers=headers_umm_var,
-                            timeout=10)
+    response = requests.put(
+        url_endpoint, json=umm_var_dict, headers=headers_umm_var, timeout=10
+    )
 
     if response.ok:
         # A successful request returns the variable concept-id
         # e.g., 'V1259791517-EEDTEST'
         return response.json()['concept-id']
     else:
         # A failed request returns the response containing a list of error
         # message, e.g., {'errors': ['#: required key [LongName] not found']}.
         # This will be converted into a single string that can be returned to
         # the end-user. Multiple errors will be combined into a single string,
         # e.g.: '#: CMR error 1\n  #: CMR error 2'
         return '\n  '.join(response.json()['errors'])
 
 
-def publish_all_umm_var(collection_id: str,
-                        all_umm_var_dict: Dict,
-                        auth_header: str,
-                        cmr_env: CmrEnvType = CMR_UAT) -> Dict[str, str]:
-    """ Publish all UMM-Var entries associated with a collection to CMR given:
+def publish_all_umm_var(
+    collection_id: str,
+    all_umm_var_dict: Dict,
+    auth_header: str,
+    cmr_env: CmrEnvType = CMR_UAT,
+) -> Dict[str, str]:
+    """Publish all UMM-Var entries associated with a collection to CMR given:
         * collection_id: a collection's concept_id
         * all_umm_var_dict: a nested dictionary containing
             dictionaries of all UMM-Var entries for a collection
         * auth_header: Authorization HTTP header, containing a LaunchPad
           token: 'Authorization: <token>'
         * cmr_env: CMR environments (OPS, UAT, and SIT)
     For a successful requests all of these fields must be entered
```

### Comparing `earthdata-varinfo-2.2.0/varinfo/utilities.py` & `earthdata-varinfo-2.2.1/varinfo/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,99 +13,126 @@
     - Section 7.5: geometry, interior_ring, node_coordinates, node_count,
                    nodes, part_node_count
 
     susbset_control_variables is a new attribute introduced by the Data
     Services team, primarily for use with references for segmented data.
 
 """
+
 from typing import Dict, List, Optional
 from xml.etree.ElementTree import Element
 import functools
 import re
 
 import numpy as np
 
 from varinfo.exceptions import DmrNamespaceError
 
 
-CF_REFERENCE_ATTRIBUTES = ['ancillary_variables', 'bounds', 'cell_measures',
-                           'coordinates', 'geometry', 'grid_mapping',
-                           'interior_ring', 'node_coordinates', 'node_count',
-                           'nodes', 'part_node_count',
-                           'subset_control_variables']
-
-DAP4_TO_NUMPY_MAP = {'Char': np.uint8, 'Byte': np.uint8, 'Int8': np.int8,
-                     'UInt8': np.uint8, 'Int16': np.int16, 'UInt16': np.uint16,
-                     'Int32': np.int32, 'UInt32': np.uint32, 'Int64': np.int64,
-                     'UInt64': np.uint64, 'Float32': np.float32,
-                     'Float64': np.float64, 'String': str, 'URL': str}
+CF_REFERENCE_ATTRIBUTES = [
+    'ancillary_variables',
+    'bounds',
+    'cell_measures',
+    'coordinates',
+    'geometry',
+    'grid_mapping',
+    'interior_ring',
+    'node_coordinates',
+    'node_count',
+    'nodes',
+    'part_node_count',
+    'subset_control_variables',
+]
+
+DAP4_TO_NUMPY_MAP = {
+    'Char': np.uint8,
+    'Byte': np.uint8,
+    'Int8': np.int8,
+    'UInt8': np.uint8,
+    'Int16': np.int16,
+    'UInt16': np.uint16,
+    'Int32': np.int32,
+    'UInt32': np.uint32,
+    'Int64': np.int64,
+    'UInt64': np.uint64,
+    'Float32': np.float32,
+    'Float64': np.float64,
+    'String': str,
+    'URL': str,
+}
 
 
 def recursive_get(input_dictionary: Dict, keys: List[str]):
-    """ Extract a value from an aribtrarily nested dictionary. """
+    """Extract a value from an aribtrarily nested dictionary."""
     try:
         nested_value = functools.reduce(dict.get, keys, input_dictionary)
     except TypeError:
         # This catches when there is a missing intermediate key
         nested_value = None
 
     return nested_value
 
 
 def split_attribute_path(full_path: str) -> List[str]:
-    """ Take the full path to a metadata attribute and return the list of
-        keys that locate that attribute within the global attributes.
-        This function can account for the input path to having, or omitting, a
-        leading '/' character.
+    """Take the full path to a metadata attribute and return the list of
+    keys that locate that attribute within the global attributes.
+    This function can account for the input path to having, or omitting, a
+    leading '/' character.
 
     """
     return full_path.lstrip('/').split('/')
 
 
 def get_xml_namespace(root_element: Element) -> str:
-    """ Given the root element of an XML document, extract the associated
-        namespace. This allows for the full qualification of child elements.
-        The root element of a dmr file is expected to be a Dataset tag.
+    """Given the root element of an XML document, extract the associated
+    namespace. This allows for the full qualification of child elements.
+    The root element of a dmr file is expected to be a Dataset tag.
 
     """
     match = re.match('(.+)Dataset', root_element.tag)
 
     if match:
         xml_namespace = match.groups()[0]
     else:
         raise DmrNamespaceError(root_element.tag)
 
     return xml_namespace
 
 
-def get_xml_attribute(variable: Element, attribute_name: str, namespace: str,
-                      default_value: Optional = None) -> Optional:
-    """ Extract the value of an XML Attribute tag from a `.dmr`. First search
-        the supplied variable element for a fully qualified Attribute child
-        element, with a name property matching the requested attribute name. If
-        there is no matching tag, return the `default_value`, which can be
-        user-defined, or default to `None`. If present, the returned value is
-        cast as the type indicated by the Attribute tag's `type` property.
+def get_xml_attribute(
+    variable: Element,
+    attribute_name: str,
+    namespace: str,
+    default_value: Optional = None,
+) -> Optional:
+    """Extract the value of an XML Attribute tag from a `.dmr`. First search
+    the supplied variable element for a fully qualified Attribute child
+    element, with a name property matching the requested attribute name. If
+    there is no matching tag, return the `default_value`, which can be
+    user-defined, or default to `None`. If present, the returned value is
+    cast as the type indicated by the Attribute tag's `type` property.
 
-        Attributes with multiple Value children will return a list of all those
-        children, cast as the indicated type.
+    Attributes with multiple Value children will return a list of all those
+    children, cast as the indicated type.
 
     """
-    attribute_element = variable.find(f'{namespace}Attribute'
-                                      f'[@name="{attribute_name}"]')
+    attribute_element = variable.find(
+        f'{namespace}Attribute' f'[@name="{attribute_name}"]'
+    )
 
     if attribute_element is not None:
         value_type = attribute_element.get('type', 'String')
         numpy_type = DAP4_TO_NUMPY_MAP.get(value_type, str)
 
         value_elements = attribute_element.findall(f'{namespace}Value')
 
         if len(value_elements) > 1:
-            attribute_value = [numpy_type(value_element.text)
-                               for value_element in value_elements]
+            attribute_value = [
+                numpy_type(value_element.text) for value_element in value_elements
+            ]
         elif len(value_elements) == 1:
             attribute_value = numpy_type(value_elements[0].text)
         else:
             attribute_value = default_value
 
     else:
         attribute_value = default_value
```

### Comparing `earthdata-varinfo-2.2.0/varinfo/var_info.py` & `earthdata-varinfo-2.2.1/varinfo/var_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,63 @@
 """ This module contains a class designed to read information from a `.dmr`
     file. This should group the input into science variables, metadata,
     coordinates, dimensions and ancillary data sets.
 
 """
+
 from abc import ABC, abstractmethod
 from os.path import exists
 from typing import Dict, Optional, Set, Tuple, Union
 import json
 import re
 import xml.etree.ElementTree as ET
 
 from netCDF4 import Dataset, Group
 
 from varinfo.cf_config import CFConfig
-from varinfo.exceptions import (InvalidConfigFileFormatError,
-                                MissingConfigurationFileError)
-from varinfo.utilities import (DAP4_TO_NUMPY_MAP, get_xml_namespace,
-                               split_attribute_path, recursive_get)
+from varinfo.exceptions import (
+    InvalidConfigFileFormatError,
+    MissingConfigurationFileError,
+)
+from varinfo.utilities import (
+    DAP4_TO_NUMPY_MAP,
+    get_xml_namespace,
+    split_attribute_path,
+    recursive_get,
+)
 from varinfo.variable import VariableFromDmr, VariableFromNetCDF4
 
 
 DimensionsGroupType = Dict[Tuple[str], Set[str]]
 OutputVariableType = Union[VariableFromDmr]
 
 
 class VarInfoBase(ABC):
-    """ An abstract base class to represent the full dataset of a granule,
-        having reading information from a representation of that granule.
+    """An abstract base class to represent the full dataset of a granule,
+    having reading information from a representation of that granule.
 
-        A class to represent the full dataset of a granule, by parsing a `.dmr`
-        file from OPeNDAP.
+    A class to represent the full dataset of a granule, by parsing a `.dmr`
+    file from OPeNDAP.
 
     """
-    def __init__(self, file_path: str, short_name: Optional[str] = None,
-                 config_file: Optional[str] = None):
-        """ Distinguish between variables containing references to other
-            datasets, and those that do not. The former are considered science
-            variables, providing they are not considered coordinates or
-            dimensions for another variable.
-
-            Each variable contains references to their specific coordinates and
-            dimensions, allowing the retrieval of all required variables for a
-            specified list of science variables.
+
+    def __init__(
+        self,
+        file_path: str,
+        short_name: Optional[str] = None,
+        config_file: Optional[str] = None,
+    ):
+        """Distinguish between variables containing references to other
+        datasets, and those that do not. The former are considered science
+        variables, providing they are not considered coordinates or
+        dimensions for another variable.
+
+        Each variable contains references to their specific coordinates and
+        dimensions, allowing the retrieval of all required variables for a
+        specified list of science variables.
 
         """
         self.config_file = config_file
         self.cf_config = None
         self.global_attributes = {}
         self.short_name = short_name
         self.mission = None
@@ -60,260 +72,261 @@
         self._set_mission_and_short_name()
         self._set_cf_config()
         self._update_global_attributes()
         self._extract_variables()
 
     @abstractmethod
     def _read_dataset(self, file_path: str):
-        """ This method parses a file at the specified location using
-            functionality specific to the type of input (e.g. a `.dmr` file).
+        """This method parses a file at the specified location using
+        functionality specific to the type of input (e.g. a `.dmr` file).
 
         """
 
     @abstractmethod
     def _set_global_attributes(self):
-        """ Extract the global attributes from the granule representation using
-            functionality specific to the type of input.
+        """Extract the global attributes from the granule representation using
+        functionality specific to the type of input.
 
         """
 
     @abstractmethod
     def _extract_variables(self):
-        """ Iterate through all variables in the retrieved dataset. For each
-            variable create an instance of a `Variable` (using the relevant
-            child class), and assign it to either the `metadata_variables`
-            or the `variable_with_coordinates` dictionary accordingly.
+        """Iterate through all variables in the retrieved dataset. For each
+        variable create an instance of a `Variable` (using the relevant
+        child class), and assign it to either the `metadata_variables`
+        or the `variable_with_coordinates` dictionary accordingly.
 
         """
 
     def _assign_variable(self, variable_object):
-        """ Save the `Variable` instance in the dictionary containing all
-            variables. Additionally, the set of references for all variables is
-            updated.
+        """Save the `Variable` instance in the dictionary containing all
+        variables. Additionally, the set of references for all variables is
+        updated.
 
         """
         full_path = variable_object.full_name_path
         self.references.update(variable_object.get_references())
         self.variables[full_path] = variable_object
 
     def _set_var_info_config(self):
-        """ Read the VarInfo configuration JSON file, containing locations to
-            search for the collection short_name attribute, and the mapping
-            from short_name to satellite mission.
+        """Read the VarInfo configuration JSON file, containing locations to
+        search for the collection short_name attribute, and the mapping
+        from short_name to satellite mission.
 
         """
         if self.config_file is not None and not exists(self.config_file):
             raise MissingConfigurationFileError(self.config_file)
-        elif (
-            self.config_file is not None and self.config_file.endswith('.json')
-        ):
+        elif self.config_file is not None and self.config_file.endswith('.json'):
             with open(self.config_file, 'r', encoding='utf-8') as file_handler:
                 self.var_info_config = json.load(file_handler)
         elif self.config_file is not None:
             raise InvalidConfigFileFormatError(self.config_file)
         else:
             self.var_info_config = {}
 
     def _set_cf_config(self):
-        """ Instantiate a CFConfig object, to contain any rules for exclusions,
-            required fields and augmentations to CF attributes that are not
-            contained within a granule from the specified collection.
+        """Instantiate a CFConfig object, to contain any rules for exclusions,
+        required fields and augmentations to CF attributes that are not
+        contained within a granule from the specified collection.
 
         """
-        self.cf_config = CFConfig(self.mission, self.short_name,
-                                  self.config_file)
+        self.cf_config = CFConfig(self.mission, self.short_name, self.config_file)
 
     def _set_mission_and_short_name(self):
-        """ Check a series of potential locations for the collection short name
+        """Check a series of potential locations for the collection short name
         of the granule. Once that is determined, match that short name to its
         associated mission.
 
         """
         if self.short_name is None:
             self.short_name = next(
-                (recursive_get(self.global_attributes,
-                               split_attribute_path(item))
-                 for item
-                 in self.var_info_config.get('Collection_ShortName_Path', [])
-                 if recursive_get(self.global_attributes,
-                                  split_attribute_path(item))
-                 is not None),
-                None
+                (
+                    recursive_get(self.global_attributes, split_attribute_path(item))
+                    for item in self.var_info_config.get(
+                        'Collection_ShortName_Path', []
+                    )
+                    if recursive_get(self.global_attributes, split_attribute_path(item))
+                    is not None
+                ),
+                None,
             )
 
         if self.short_name is not None:
-            self.mission = next((name
-                                 for pattern, name
-                                 in self.var_info_config.get('Mission', {}).items()
-                                 if re.match(pattern, self.short_name)
-                                 is not None), None)
+            self.mission = next(
+                (
+                    name
+                    for pattern, name in self.var_info_config.get('Mission', {}).items()
+                    if re.match(pattern, self.short_name) is not None
+                ),
+                None,
+            )
 
     def _update_global_attributes(self):
-        """ Having identified the mission and short_name for the granule, and
-            therefore obtained the relevant CF configuration overrides and
-            supplements, update the global attributes for this granule using
-            the CFConfig class instance. As the overrides are assumed to have
-            the strongest priority, the dictionary is updated with these values
-            last.
+        """Having identified the mission and short_name for the granule, and
+        therefore obtained the relevant CF configuration overrides and
+        supplements, update the global attributes for this granule using
+        the CFConfig class instance. As the overrides are assumed to have
+        the strongest priority, the dictionary is updated with these values
+        last.
 
         """
         if self.cf_config.global_supplements:
             self.global_attributes.update(self.cf_config.global_supplements)
 
         if self.cf_config.global_overrides:
             self.global_attributes.update(self.cf_config.global_overrides)
 
     def get_variable(self, variable_path: str) -> Optional[OutputVariableType]:
-        """ Retrieve a variable specified by an absolute path. First check the
-            variables with coordinates, before checking those without. If there
-            are no matching variables, a value of `None` is returned.
+        """Retrieve a variable specified by an absolute path. First check the
+        variables with coordinates, before checking those without. If there
+        are no matching variables, a value of `None` is returned.
 
         """
         return self.variables.get(variable_path)
 
     def get_all_variables(self) -> Set[str]:
-        """ Retrieve a set of names for all variables in the granule. """
+        """Retrieve a set of names for all variables in the granule."""
         return set(self.variables.keys())
 
     def get_variables_with_coordinates(self) -> Dict[str, OutputVariableType]:
-        """ Return only variables with a `coordinates` metadata attribute.
-            This list excludes any variables listed as an excluded science
-            variable in the configuration file supplied to the object.
+        """Return only variables with a `coordinates` metadata attribute.
+        This list excludes any variables listed as an excluded science
+        variable in the configuration file supplied to the object.
 
         """
         exclusion_pattern = re.compile(
             '|'.join(self.cf_config.excluded_science_variables)
         )
 
-        return {variable_path: variable
-                for variable_path, variable in self.variables.items()
-                if variable.references.get('coordinates') is not None
-                and not self.variable_is_excluded(variable, exclusion_pattern)}
+        return {
+            variable_path: variable
+            for variable_path, variable in self.variables.items()
+            if variable.references.get('coordinates') is not None
+            and not self.variable_is_excluded(variable, exclusion_pattern)
+        }
 
     def _is_spatial_temporal_dimension(self, dimension_path: str) -> bool:
-        """ A helper method simplifying the list comprehension in
-            `is_science_variable`.
+        """A helper method simplifying the list comprehension in
+        `is_science_variable`.
         """
         dimension = self.get_variable(dimension_path)
         return dimension is not None and (
             dimension.is_geographic()
             or dimension.is_temporal()
             or dimension.is_projection_x_or_y()
         )
 
     def is_science_variable(self, variable: OutputVariableType) -> bool:
-        """ Determine if a variable is a science variable.
-            A science variable is classified as a variable that is NOT
-            a spatial temporal dimension variable. But contains
-            geographic, temporal, and or projected spatial dimensions, or
-            a coordinate or grid mapping reference attribute.
+        """Determine if a variable is a science variable.
+        A science variable is classified as a variable that is NOT
+        a spatial temporal dimension variable. But contains
+        geographic, temporal, and or projected spatial dimensions, or
+        a coordinate or grid mapping reference attribute.
 
         """
         if any(
             self._is_spatial_temporal_dimension(dimension)
             for dimension in variable.dimensions
             if dimension != variable.full_name_path
             and not variable.full_name_path.endswith('_bnds')
         ):
             return True
 
         if (
-                variable.references.get('coordinates') is not None
-                or variable.references.get('grid_mapping') is not None
+            variable.references.get('coordinates') is not None
+            or variable.references.get('grid_mapping') is not None
         ):
             return True
 
         return False
 
     def get_science_variables(self) -> Set[str]:
-        """ Retrieve a set of names for all variables that have coordinate
-            references, that are not themselves used as dimensions, coordinates
-            or ancillary date for another variable.
+        """Retrieve a set of names for all variables that have coordinate
+        references, that are not themselves used as dimensions, coordinates
+        or ancillary date for another variable.
 
         """
         exclusions_pattern = re.compile(
             '|'.join(self.cf_config.excluded_science_variables)
         )
 
         filtered_with_coordinates = {
             variable_path
-            for variable_path, variable
-            in self.variables.items()
+            for variable_path, variable in self.variables.items()
             if variable_path is not None
             and self.is_science_variable(variable)
-            and not self.variable_is_excluded(variable_path,
-                                              exclusions_pattern)
+            and not self.variable_is_excluded(variable_path, exclusions_pattern)
         }
 
         return filtered_with_coordinates - self.references
 
     def get_metadata_variables(self) -> Set[str]:
-        """ Retrieve set of names for all variables that do no have
-            coordinates references, that are not themselves used as dimensions,
-            coordinates, ancillary data for another variable, or are
-            science variables.
-
-            Additionally, any excluded science variables, that are contained
-            in the variables class attribute should be considered a metadata
-            variable.
+        """Retrieve set of names for all variables that do no have
+        coordinates references, that are not themselves used as dimensions,
+        coordinates, ancillary data for another variable, or are
+        science variables.
+
+        Additionally, any excluded science variables, that are contained
+        in the variables class attribute should be considered a metadata
+        variable.
 
         """
         exclusions_pattern = re.compile(
             '|'.join(self.cf_config.excluded_science_variables)
         )
 
         non_coordinate_variables = {
             variable_path
-            for variable_path, variable
-            in self.variables.items()
+            for variable_path, variable in self.variables.items()
             if variable_path is not None
             and (
                 not self.variable_is_excluded(variable_path, exclusions_pattern)
                 and not self.is_science_variable(variable)
                 and not variable.full_name_path.endswith('_bnds')
             )
         }
 
         return non_coordinate_variables - self.references
 
     @staticmethod
-    def variable_is_excluded(variable_name: str,
-                             exclusions_pattern: re.Pattern) -> bool:
-        """ Ensure the variable name does not match any collection specific
-            exclusion rules.
+    def variable_is_excluded(
+        variable_name: str, exclusions_pattern: re.Pattern
+    ) -> bool:
+        """Ensure the variable name does not match any collection specific
+        exclusion rules.
 
         """
         if exclusions_pattern.pattern != '':
             exclude_variable = exclusions_pattern.match(variable_name) is not None
         else:
             exclude_variable = False
 
         return exclude_variable
 
     def get_required_variables(self, requested_variables: Set[str]) -> Set[str]:
-        """ Retrieve requested variables and recursively search for all
-            associated dimension and coordinate variables. The returned set
-            should be the union of the science variables, coordinates and
-            dimensions.
-
-            The requested variables are also augmented to include required
-            variables for the collection, as indicated by the CFConfig class
-            instance, and any references within those variables.
+        """Retrieve requested variables and recursively search for all
+        associated dimension and coordinate variables. The returned set
+        should be the union of the science variables, coordinates and
+        dimensions.
+
+        The requested variables are also augmented to include required
+        variables for the collection, as indicated by the CFConfig class
+        instance, and any references within those variables.
 
         """
         if self.cf_config.required_variables:
             cf_required_pattern = re.compile(
                 '|'.join(self.cf_config.required_variables)
             )
 
-            cf_required_variables = {variable
-                                     for variable
-                                     in self.get_all_variables()
-                                     if variable is not None
-                                     and re.match(cf_required_pattern, variable)}
+            cf_required_variables = {
+                variable
+                for variable in self.get_all_variables()
+                if variable is not None and re.match(cf_required_pattern, variable)
+            }
         else:
             cf_required_variables = set()
 
         requested_variables.update(cf_required_variables)
         required_variables: Set[str] = set()
 
         while len(requested_variables) > 0:
@@ -324,142 +337,149 @@
 
             if variable is not None:
                 # Add variable. Enqueue references not already present in
                 # required set. (Also checking that they are real variables,
                 # and not non-variable dimensions)
                 variable_references = {
                     reference_variable
-                    for reference_variable
-                    in variable.get_references()
+                    for reference_variable in variable.get_references()
                     if self.get_variable(reference_variable) is not None
                 }
                 requested_variables.update(
                     variable_references.difference(required_variables)
                 )
 
         return self.exclude_fake_dimensions(required_variables)
 
     def get_required_dimensions(self, variables: Set[str]) -> Set[str]:
-        """ Return a single set of all variables that are used as dimensions
-            for any of the listed variables.
+        """Return a single set of all variables that are used as dimensions
+        for any of the listed variables.
 
         """
-        return set(dimension
-                   for variable in variables
-                   for dimension
-                   in getattr(self.get_variable(variable), 'dimensions', [])
-                   if self.get_variable(dimension) is not None)
+        return set(
+            dimension
+            for variable in variables
+            for dimension in getattr(self.get_variable(variable), 'dimensions', [])
+            if self.get_variable(dimension) is not None
+        )
 
     def get_spatial_dimensions(self, variables: Set[str]) -> Set[str]:
-        """ Return a single set of all variables that are both used as
-            dimensions for any of the input variables, and that are horizontal
-            spatial dimensions (either geographic or projected).
+        """Return a single set of all variables that are both used as
+        dimensions for any of the input variables, and that are horizontal
+        spatial dimensions (either geographic or projected).
 
         """
-        return set().union(self.get_geographic_spatial_dimensions(variables),
-                           self.get_projected_spatial_dimensions(variables))
+        return set().union(
+            self.get_geographic_spatial_dimensions(variables),
+            self.get_projected_spatial_dimensions(variables),
+        )
 
-    def get_geographic_spatial_dimensions(self,
-                                          variables: Set[str]) -> Set[str]:
-        """ Return a single set of all the variables that are both used as
-            dimensions for any of the input variables, and that are geographic
-            in nature (as determined by the `units` metadata attribute).
+    def get_geographic_spatial_dimensions(self, variables: Set[str]) -> Set[str]:
+        """Return a single set of all the variables that are both used as
+        dimensions for any of the input variables, and that are geographic
+        in nature (as determined by the `units` metadata attribute).
 
-            Not all variables have dimensions, which necessitates a check on
-            their existence before determining the dimension is geographic.
+        Not all variables have dimensions, which necessitates a check on
+        their existence before determining the dimension is geographic.
 
         """
-        return set(dimension
-                   for dimension
-                   in self.get_required_dimensions(variables)
-                   if self.get_variable(dimension).is_geographic())
+        return set(
+            dimension
+            for dimension in self.get_required_dimensions(variables)
+            if self.get_variable(dimension).is_geographic()
+        )
 
-    def get_projected_spatial_dimensions(self,
-                                         variables: Set[str]) -> Set[str]:
-        """ Return a single set of all the variables that are both used as
-            dimensions for any of the input variables, and that are projected
-            in nature (as determined by the `standard_name` metadata
-            attribute).
+    def get_projected_spatial_dimensions(self, variables: Set[str]) -> Set[str]:
+        """Return a single set of all the variables that are both used as
+        dimensions for any of the input variables, and that are projected
+        in nature (as determined by the `standard_name` metadata
+        attribute).
 
         """
-        return set(dimension
-                   for dimension
-                   in self.get_required_dimensions(variables)
-                   if self.get_variable(dimension).is_projection_x_or_y())
+        return set(
+            dimension
+            for dimension in self.get_required_dimensions(variables)
+            if self.get_variable(dimension).is_projection_x_or_y()
+        )
 
     def get_temporal_dimensions(self, variables: Set[str]) -> Set[str]:
-        """ Return a single set of all variables that are both used as
-            dimensions for any of the input variables, and that are temporal
-            in nature (as determined by the `units` metadata attribute).
-
-            Not all variables have dimensions, which necessitates a check on
-            their existence before determining the dimension is temporal.
+        """Return a single set of all variables that are both used as
+        dimensions for any of the input variables, and that are temporal
+        in nature (as determined by the `units` metadata attribute).
+
+        Not all variables have dimensions, which necessitates a check on
+        their existence before determining the dimension is temporal.
 
         """
-        return set(dimension
-                   for dimension
-                   in self.get_required_dimensions(variables)
-                   if self.get_variable(dimension).is_temporal())
+        return set(
+            dimension
+            for dimension in self.get_required_dimensions(variables)
+            if self.get_variable(dimension).is_temporal()
+        )
 
     def get_variables_with_dimensions(self, dimensions: Set[str]) -> Set[str]:
-        """ Return a single set of all variables that include all the supplied
-            dimensions as a subset of their own dimensions.
+        """Return a single set of all variables that include all the supplied
+        dimensions as a subset of their own dimensions.
 
         """
         return set(
-            variable for variable in self.get_all_variables()
+            variable
+            for variable in self.get_all_variables()
             if dimensions.issubset(set(self.get_variable(variable).dimensions))
         )
 
     def group_variables_by_dimensions(self) -> DimensionsGroupType:
-        """ Retrieve a dictionary that groups all variables in a file by the
-            dimensions for their arrays. Example output for M2I3NPASM:
+        """Retrieve a dictionary that groups all variables in a file by the
+        dimensions for their arrays. Example output for M2I3NPASM:
 
-            ```
-            {
-                ('/time', '/lev', '/lat', '/lon'): {'/EPV', '/H', ...},
-                ('/time', '/lat', '/lon'): {'/PHIS', '/PS', '/SLP'},
-                ('/lev', ): {'/lev', },
-                ('/lat', ): {'/lat', },
-                ('/lon', ): {'/lon', },
-                ('/time', ): {'/time', },
-            }
-            ```
+        ```
+        {
+            ('/time', '/lev', '/lat', '/lon'): {'/EPV', '/H', ...},
+            ('/time', '/lat', '/lon'): {'/PHIS', '/PS', '/SLP'},
+            ('/lev', ): {'/lev', },
+            ('/lat', ): {'/lat', },
+            ('/lon', ): {'/lon', },
+            ('/time', ): {'/time', },
+        }
+        ```
 
         """
         grouped_variables = {}
 
         for variable_name in self.get_all_variables():
             variable = self.get_variable(variable_name)
             variable_dimensions = tuple(variable.dimensions)
 
             if variable_dimensions in grouped_variables:
                 grouped_variables[variable_dimensions].add(variable_name)
             else:
-                grouped_variables[variable_dimensions] = {variable_name, }
+                grouped_variables[variable_dimensions] = {
+                    variable_name,
+                }
 
         return grouped_variables
 
     def group_variables_by_horizontal_dimensions(self) -> DimensionsGroupType:
-        """ Retrieve a dictionary that groups all variables by shared
-            horizontal spatial dimensions (e.g., (lon, lat) or (x, y)),
-            regardless of other dimensions. This will, for example, group
-            variables with dimensions (time, lat, lon) with variables only
-            having dimensions (lat, lon). Note, though, the ordering is
-            considered, so variables with dimensions (lat, lon) will not be
-            grouped with variables having dimensions (lon, lat).
+        """Retrieve a dictionary that groups all variables by shared
+        horizontal spatial dimensions (e.g., (lon, lat) or (x, y)),
+        regardless of other dimensions. This will, for example, group
+        variables with dimensions (time, lat, lon) with variables only
+        having dimensions (lat, lon). Note, though, the ordering is
+        considered, so variables with dimensions (lat, lon) will not be
+        grouped with variables having dimensions (lon, lat).
 
         """
         grid_groups = self.group_variables_by_dimensions()
 
         horizontal_groups = {}
 
         for grid_dimensions, variables in grid_groups.items():
             horizontal_dimensions = tuple(
-                dimension for dimension in grid_dimensions
+                dimension
+                for dimension in grid_dimensions
                 if (
                     self.get_variable(dimension) is not None
                     and (
                         self.get_variable(dimension).is_geographic()
                         or self.get_variable(dimension).is_projection_x_or_y()
                     )
                 )
@@ -470,52 +490,55 @@
             else:
                 horizontal_groups[horizontal_dimensions] = variables
 
         return horizontal_groups
 
     @staticmethod
     def exclude_fake_dimensions(variable_set: Set[str]) -> Set[str]:
-        """ An OPeNDAP `.dmr` can contain fake dimensions, used to supplement
-            missing information for a granule. These cannot be retrieved when
-            requesting a subset from an OPeNDAP server, and must be removed
-            from the list of required variables.
+        """An OPeNDAP `.dmr` can contain fake dimensions, used to supplement
+        missing information for a granule. These cannot be retrieved when
+        requesting a subset from an OPeNDAP server, and must be removed
+        from the list of required variables.
 
         """
         fakedim_pattern = re.compile(r'.*/FakeDim\d+')
 
-        return {variable for variable in variable_set
-                if not fakedim_pattern.match(variable)}
+        return {
+            variable for variable in variable_set if not fakedim_pattern.match(variable)
+        }
 
 
 class VarInfoFromDmr(VarInfoBase):
-    """ A child class that inherits from `VarInfoBase` and implements functions
-        to retrieve a dataset from a `.dmr` file, and the extract variables
-        from the resulting XML tree.
+    """A child class that inherits from `VarInfoBase` and implements functions
+    to retrieve a dataset from a `.dmr` file, and the extract variables
+    from the resulting XML tree.
 
     """
+
     def _read_dataset(self, file_path: str):
-        """ Extract the XML tree and namespace from an OPeNDAP `.dmr` file. """
+        """Extract the XML tree and namespace from an OPeNDAP `.dmr` file."""
         with open(file_path, 'r', encoding='utf-8') as file_handler:
             dmr_content = file_handler.read()
 
         self.dataset = ET.fromstring(dmr_content)
         self.namespace = get_xml_namespace(self.dataset)
 
     def _set_global_attributes(self):
-        """ Extract all global attributes from a `.dmr` file. First this method
-            searches for a root level Attribute element with name
-            "HDF5_GLOBAL". If this is present, it is assumed to be a container
-            for the global attributes. If "HDF5_GLOBAL" is absent, the global
-            attributes are assumed to be direct children of the root Dataset
-            element in the XML tree. All child Attribute elements children with
-            a type property corresponding to a DAP4 variable type are placed in
-            an output dictionary. If the type is not recognised by the DAP4
-            protocol, the attribute is assumed to be a string.
+        """Extract all global attributes from a `.dmr` file. First this method
+        searches for a root level Attribute element with name
+        "HDF5_GLOBAL". If this is present, it is assumed to be a container
+        for the global attributes. If "HDF5_GLOBAL" is absent, the global
+        attributes are assumed to be direct children of the root Dataset
+        element in the XML tree. All child Attribute elements children with
+        a type property corresponding to a DAP4 variable type are placed in
+        an output dictionary. If the type is not recognised by the DAP4
+        protocol, the attribute is assumed to be a string.
 
         """
+
         def save_attribute(output, group_path, attribute):
             attribute_name = attribute.get('name')
             dap4_type = attribute.get('type')
 
             if dap4_type != 'Container':
                 attribute_value = attribute.find(f'{self.namespace}Value').text
                 numpy_type = DAP4_TO_NUMPY_MAP.get(dap4_type, str)
@@ -530,121 +553,140 @@
                     # dictionary for the group to contain the child attributes
                     nested_groups = group_path.lstrip('/').split('/')
                     for group in nested_groups:
                         group_dictionary = group_dictionary.setdefault(group, {})
 
                 group_dictionary[attribute_name] = numpy_type(attribute_value)
 
-        globals_parent = self.dataset.find(
-            f'{self.namespace}Attribute[@name="HDF5_GLOBAL"]'
-        ) or self.dataset
+        globals_parent = (
+            self.dataset.find(f'{self.namespace}Attribute[@name="HDF5_GLOBAL"]')
+            or self.dataset
+        )
 
-        self.traverse_elements(globals_parent, {'Attribute'}, save_attribute,
-                               self.global_attributes)
+        self.traverse_elements(
+            globals_parent, {'Attribute'}, save_attribute, self.global_attributes
+        )
 
     def _extract_variables(self):
-        """ Iterate through all children of the `.dmr` root dataset element.
-            If the child matches one of the DAP4 variable types, then create an
-            instance of the `VariableFromDmr` class, and assign it to either
-            the `variables_with_coordinates` or the `metadata_variables`
-            dictionary accordingly.
+        """Iterate through all children of the `.dmr` root dataset element.
+        If the child matches one of the DAP4 variable types, then create an
+        instance of the `VariableFromDmr` class, and assign it to either
+        the `variables_with_coordinates` or the `metadata_variables`
+        dictionary accordingly.
 
         """
+
         def save_variable(output, group_path, element):
             element_path = '/'.join([group_path, element.get('name')])
-            variable = VariableFromDmr(element, self.cf_config,
-                                       namespace=self.namespace,
-                                       full_name_path=element_path)
+            variable = VariableFromDmr(
+                element,
+                self.cf_config,
+                namespace=self.namespace,
+                full_name_path=element_path,
+            )
             output[variable.full_name_path] = variable
             self._assign_variable(variable)
 
         all_variables = {}
 
-        self.traverse_elements(self.dataset, set(DAP4_TO_NUMPY_MAP.keys()),
-                               save_variable, all_variables)
+        self.traverse_elements(
+            self.dataset, set(DAP4_TO_NUMPY_MAP.keys()), save_variable, all_variables
+        )
 
         self._remove_non_variable_references()
 
     def _remove_non_variable_references(self):
-        """ After all references have been combined, remove those that point to
-            non-existent variables. For example dimensions that are present in
-            a variable to only denote array size in that dimension. This must
-            be done after all variables are parsed, to ensure a reference isn't
-            being made to a variable that hasn't yet been extracted.
-
-        """
-        self.references = {reference
-                           for reference
-                           in self.references
-                           if self.get_variable(reference) is not None}
-
-    def traverse_elements(self, element: ET.Element, element_types: Set[str],
-                          operation, output, group_path: str = ''):
-        """ Perform a depth first search of the `.dmr` `Dataset` element.
-            When a variable is located perform an operation on the supplied
-            output object, using the supplied function or class.
+        """After all references have been combined, remove those that point to
+        non-existent variables. For example dimensions that are present in
+        a variable to only denote array size in that dimension. This must
+        be done after all variables are parsed, to ensure a reference isn't
+        being made to a variable that hasn't yet been extracted.
+
+        """
+        self.references = {
+            reference
+            for reference in self.references
+            if self.get_variable(reference) is not None
+        }
+
+    def traverse_elements(
+        self,
+        element: ET.Element,
+        element_types: Set[str],
+        operation,
+        output,
+        group_path: str = '',
+    ):
+        """Perform a depth first search of the `.dmr` `Dataset` element.
+        When a variable is located perform an operation on the supplied
+        output object, using the supplied function or class.
 
         """
         for child in list(element):
             # If it is in the DAP4 list: use the function
             # else, if it is a Group, call this function again
             element_type = child.tag.replace(self.namespace, '')
 
             if element_type in element_types:
                 operation(output, group_path, child)
             elif element_type == 'Group':
                 new_group_path = '/'.join([group_path, child.get('name')])
-                self.traverse_elements(child, element_types, operation, output,
-                                       new_group_path)
+                self.traverse_elements(
+                    child, element_types, operation, output, new_group_path
+                )
 
 
 class VarInfoFromNetCDF4(VarInfoBase):
-    """ A child class that inherits from `VarInfoBase` and implements functions
-        to retrieve a dataset from a NetCDF-4 file, and extract the variables
-        by traversing the granule structure.
+    """A child class that inherits from `VarInfoBase` and implements functions
+    to retrieve a dataset from a NetCDF-4 file, and extract the variables
+    by traversing the granule structure.
 
     """
+
     def _read_dataset(self, file_path: str):
-        """ Set the dataset to the file path for the NetCDF-4 file. This is
-            done instead of assigning a `netCDF4.Dataset` instance, so that the
-            file is not still in memory after being parsed, so that other
-            services can interact with the NetCDF-4 file without any conflicts.
+        """Set the dataset to the file path for the NetCDF-4 file. This is
+        done instead of assigning a `netCDF4.Dataset` instance, so that the
+        file is not still in memory after being parsed, so that other
+        services can interact with the NetCDF-4 file without any conflicts.
 
         """
         self.dataset = file_path
 
     def _set_global_attributes(self):
-        """ Extract all global attributes from the NetCDF-4 dataset. Using the
-            `Dataset.__dict__` method allows extraction of all global
-            attributes in a single call.
+        """Extract all global attributes from the NetCDF-4 dataset. Using the
+        `Dataset.__dict__` method allows extraction of all global
+        attributes in a single call.
 
         """
         with Dataset(self.dataset, 'r') as dataset:
             self.global_attributes = dataset.__dict__
 
     def _extract_variables(self):
-        """ Traverse all groups of the NetCDF-4 file, beginning at the  root
-            group.
+        """Traverse all groups of the NetCDF-4 file, beginning at the  root
+        group.
 
         """
         with Dataset(self.dataset, 'r') as dataset:
             self._parse_group(dataset)
 
     def _parse_group(self, group: Union[Dataset, Group]):
-        """ If the child matches one of the DAP4 variable types, then create an
-            instance of the `VariableFromDmr` class, and assign it to either
-            the `variables_with_coordinates` or the `metadata_variables`
-            dictionary accordingly.
+        """If the child matches one of the DAP4 variable types, then create an
+        instance of the `VariableFromDmr` class, and assign it to either
+        the `variables_with_coordinates` or the `metadata_variables`
+        dictionary accordingly.
 
         """
         for netcdf4_variable in group.variables.values():
             variable_path = '/'.join([group.path, netcdf4_variable.name])
             variable_path = f'/{variable_path.lstrip("/")}'
 
-            variable = VariableFromNetCDF4(netcdf4_variable, self.cf_config,
-                                           namespace=self.namespace,
-                                           full_name_path=variable_path)
+            variable = VariableFromNetCDF4(
+                netcdf4_variable,
+                self.cf_config,
+                namespace=self.namespace,
+                full_name_path=variable_path,
+            )
 
             self._assign_variable(variable)
 
         for child_group in group.groups.values():
             self._parse_group(child_group)
```

### Comparing `earthdata-varinfo-2.2.0/varinfo/variable.py` & `earthdata-varinfo-2.2.1/varinfo/variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ This module contains a class designed to read information from a `.dmr`
     file. This should group the input into science variables, metadata,
     coordinates, dimensions and ancillary data sets.
 
 """
+
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 import re
 import xml.etree.ElementTree as ET
 
 from netCDF4 import Variable as NetCDF4Variable
 
@@ -14,27 +15,33 @@
 from varinfo.utilities import CF_REFERENCE_ATTRIBUTES, get_xml_attribute
 
 
 InputVariableType = Union[ET.Element, NetCDF4Variable]
 
 
 class VariableBase(ABC):
-    """ A class to represent a single variable contained within a granule
-        representation. It will produce an object in which references are
-        fully qualified, and also augmented by any overrides or supplements
-        from the supplied configuration file.
+    """A class to represent a single variable contained within a granule
+    representation. It will produce an object in which references are
+    fully qualified, and also augmented by any overrides or supplements
+    from the supplied configuration file.
 
     """
-    def __init__(self, variable: InputVariableType, cf_config: CFConfig,
-                 namespace: str, full_name_path: str):
-        """ Extract the references contained within the appropriate
-            CF-Convention attributes of the variable. These should be augmented
-            by information from the `CFConfig` instance passed to the class.
 
-            Additionally, store all metadata attributes in a dictionary.
+    def __init__(
+        self,
+        variable: InputVariableType,
+        cf_config: CFConfig,
+        namespace: str,
+        full_name_path: str,
+    ):
+        """Extract the references contained within the appropriate
+        CF-Convention attributes of the variable. These should be augmented
+        by information from the `CFConfig` instance passed to the class.
+
+        Additionally, store all metadata attributes in a dictionary.
 
         """
         self.namespace = namespace
         self.full_name_path = full_name_path
         self.cf_config = cf_config.get_cf_attributes(self.full_name_path)
         self.group_path, self.name = self._extract_group_and_name()
         self.data_type = self._get_data_type(variable)
@@ -42,228 +49,242 @@
         self.attributes = self._get_attributes(variable)
         self._get_additional_attributes()
         self.references = self._get_all_cf_references()
         self.dimensions = self._extract_dimensions(variable)
 
     @abstractmethod
     def _get_data_type(self, variable: InputVariableType):
-        """ Extract a string representation of the variable data type. """
+        """Extract a string representation of the variable data type."""
 
     @abstractmethod
     def _get_shape(self, variable: InputVariableType):
-        """ Extract the shape of the variable array. """
+        """Extract the shape of the variable array."""
 
     @abstractmethod
     def _get_raw_dimensions(self, variable: InputVariableType):
-        """ Retrieve the dimension names as they are stored within the
-            variable.
+        """Retrieve the dimension names as they are stored within the
+        variable.
 
         """
 
     @abstractmethod
     def _get_attributes(self, variable: InputVariableType) -> Dict[str, str]:
-        """ Extract all attributes for the variable. The contents of the
-            output dictionary will be as stored in the granule metadata, with
-            augmentation from `CFConfig`. For variables references contained
-            in CF-Convention attributes, users should retrieve values from the
-            self.references dictionary.
+        """Extract all attributes for the variable. The contents of the
+        output dictionary will be as stored in the granule metadata, with
+        augmentation from `CFConfig`. For variables references contained
+        in CF-Convention attributes, users should retrieve values from the
+        self.references dictionary.
 
         """
 
     @abstractmethod
-    def _get_attribute(self, variable: InputVariableType,
-                       attribute_name: str) -> Any:
-        """ Extract an attribute value from the source granule metadata. Any
-            applicable overrides or supplements from `CFConfig` will be
-            applied before returning the attribute value.
+    def _get_attribute(self, variable: InputVariableType, attribute_name: str) -> Any:
+        """Extract an attribute value from the source granule metadata. Any
+        applicable overrides or supplements from `CFConfig` will be
+        applied before returning the attribute value.
 
         """
 
-    def get_attribute_value(self, attribute_name: str,
-                            default_value: Optional = None) -> Any:
-        """ A convenience function for the end-user to retrieve the value of a
-            specified attribute, or use an optional default value if that
-            attribute is not present in the variable metadata. If no default
-            value is supplied, requesting the value of an absent attribute will
-            return `None`.
+    def get_attribute_value(
+        self, attribute_name: str, default_value: Optional = None
+    ) -> Any:
+        """A convenience function for the end-user to retrieve the value of a
+        specified attribute, or use an optional default value if that
+        attribute is not present in the variable metadata. If no default
+        value is supplied, requesting the value of an absent attribute will
+        return `None`.
 
         """
         return self.attributes.get(attribute_name, default_value)
 
     def _get_additional_attributes(self) -> None:
-        """ Check the CF-Configuration file for any metadata attributes that
-            are listed, but not included in the original granule metadata.
-            These should be added to the variable metadata attributes.
+        """Check the CF-Configuration file for any metadata attributes that
+        are listed, but not included in the original granule metadata.
+        These should be added to the variable metadata attributes.
 
         """
         self._add_missing_attributes(self.cf_config.get('cf_overrides'))
         self._add_missing_attributes(self.cf_config.get('cf_supplements'))
 
     def _add_missing_attributes(self, extra_attributes: Dict) -> None:
-        """ Iterate through a dictionary of attributes from the configuration
-            file entry matching this variable. If there are any attributes
-            listed that are not already present in the self.attributes
-            dictionary, then add them with the values from the configuration
-            file.
+        """Iterate through a dictionary of attributes from the configuration
+        file entry matching this variable. If there are any attributes
+        listed that are not already present in the self.attributes
+        dictionary, then add them with the values from the configuration
+        file.
 
         """
         for attribute_name, attribute_value in extra_attributes.items():
             if attribute_name not in self.attributes:
                 self.attributes[attribute_name] = attribute_value
 
     def get_range(self) -> Optional[List[float]]:
-        """ Retrieve the range of valid data from the variable metadata. First,
-            try to parse the `valid_range` metadata attribute. If this is
-            absent, check for a combination of `valid_min` and `valid_max`.
+        """Retrieve the range of valid data from the variable metadata. First,
+        try to parse the `valid_range` metadata attribute. If this is
+        absent, check for a combination of `valid_min` and `valid_max`.
 
-            If insufficient range information is present in the metadata, this
-            method will return `None`.
+        If insufficient range information is present in the metadata, this
+        method will return `None`.
 
         """
         valid_range = self.attributes.get('valid_range')
 
         if valid_range is None:
             valid_min = self.attributes.get('valid_min')
             valid_max = self.attributes.get('valid_max')
 
             if valid_min is not None and valid_max is not None:
                 valid_range = [valid_min, valid_max]
 
         return valid_range
 
     def get_valid_min(self) -> Optional[float]:
-        """ Retrieve the minimum valid value for variable data from the
-            associated metadata. First try to retrieve data from the
-            `valid_min` metadata attribute. If this is absent, then try to
-            retrieve the same information from the `valid_range` metadata.
+        """Retrieve the minimum valid value for variable data from the
+        associated metadata. First try to retrieve data from the
+        `valid_min` metadata attribute. If this is absent, then try to
+        retrieve the same information from the `valid_range` metadata.
 
-            If insufficient range information is present in the metadata, this
-            method will return `None`.
+        If insufficient range information is present in the metadata, this
+        method will return `None`.
 
         """
         valid_min = self.attributes.get('valid_min')
 
         if valid_min is None:
             valid_range = self.attributes.get('valid_range')
             if isinstance(valid_range, list) and len(valid_range) == 2:
                 valid_min = valid_range[0]
 
         return valid_min
 
     def get_valid_max(self) -> Optional[float]:
-        """ Retrieve the maximum valid value for variable data from the
-            associated metadata. First try to retrieve data from the
-            `valid_max` metadata attribute. If this is absent, then try to
-            retrieve the same information from the `valid_range` metadata.
+        """Retrieve the maximum valid value for variable data from the
+        associated metadata. First try to retrieve data from the
+        `valid_max` metadata attribute. If this is absent, then try to
+        retrieve the same information from the `valid_range` metadata.
 
-            If insufficient range information is present in the metadata, this
-            method will return `None`.
+        If insufficient range information is present in the metadata, this
+        method will return `None`.
 
         """
         valid_max = self.attributes.get('valid_max')
 
         if valid_max is None:
             valid_range = self.attributes.get('valid_range')
             if isinstance(valid_range, list) and len(valid_range) == 2:
                 valid_max = valid_range[1]
 
         return valid_max
 
     def get_references(self) -> Set[str]:
-        """ Combine the references extracted from the ancillary_variables,
-            coordinates and dimensions data into a single set for VarInfo to
-            use directly.
-
-            The variable dimensions are cast as a set to allow combination with
-            the other set attributes of the `VariableBase` class. The
-            dimensions attribute is kept as a list prior to combination in the
-            full set of variable references to ensure that the ordering of the
-            dimensions is preserved.
+        """Combine the references extracted from the ancillary_variables,
+        coordinates and dimensions data into a single set for VarInfo to
+        use directly.
+
+        The variable dimensions are cast as a set to allow combination with
+        the other set attributes of the `VariableBase` class. The
+        dimensions attribute is kept as a list prior to combination in the
+        full set of variable references to ensure that the ordering of the
+        dimensions is preserved.
 
         """
         return set(self.dimensions).union(*self.references.values())
 
     def is_geographic(self) -> bool:
-        """ Use heuristics to determine if the variable is a geographic
-            coordinate based on its units. A latitude variable will have units
-            'degrees_north' and a longitude variable with have units
-            'degrees_east'.
+        """Use heuristics to determine if the variable is a geographic
+        coordinate based on its units. A latitude variable will have units
+        'degrees_north' and a longitude variable with have units
+        'degrees_east'.
 
         """
         return self.is_longitude() or self.is_latitude()
 
     def is_latitude(self) -> bool:
-        """ Determine if the variable is a latitude based on the `units`
-            metadata attribute being 'degrees_north' or other similar options
-            as defined in section 4.1 of the CF Conventions (v1.8).
+        """Determine if the variable is a latitude based on the `units`
+        metadata attribute being 'degrees_north' or other similar options
+        as defined in section 4.1 of the CF Conventions (v1.8).
 
         """
-        return self.attributes.get('units') in ['degrees_north',
-                                                'degree_north',
-                                                'degrees_N', 'degree_N',
-                                                'degreesN', 'degreeN']
+        return self.attributes.get('units') in [
+            'degrees_north',
+            'degree_north',
+            'degrees_N',
+            'degree_N',
+            'degreesN',
+            'degreeN',
+        ]
 
     def is_longitude(self) -> bool:
-        """ Determine if the variable is a longitude based on the `units`
-            metadata attribute being 'degrees_east' or other similar options
-            as defined in section 4.2 of the CF Conventions (v1.8).
+        """Determine if the variable is a longitude based on the `units`
+        metadata attribute being 'degrees_east' or other similar options
+        as defined in section 4.2 of the CF Conventions (v1.8).
 
         """
-        return self.attributes.get('units') in ['degrees_east', 'degree_east',
-                                                'degrees_E', 'degree_E',
-                                                'degreesE', 'degreeE']
+        return self.attributes.get('units') in [
+            'degrees_east',
+            'degree_east',
+            'degrees_E',
+            'degree_E',
+            'degreesE',
+            'degreeE',
+        ]
 
     def is_projection_x_or_y(self) -> bool:
-        """ Determine if the variable is a projected x or y horizontal spatial
-            coordinate based on the `standard_name` metadata attribute being
-            `projection_x_coordinate` or `projection_y_coordinate`, as defined
-            by the CF Conventions (v1.9). Note, geostationary projections have
-            coordinates with `standard_name` metadata attribute values of
-            `projection_x_angular_coordinate` and
-            `projection_y_angular_coordinate`.
+        """Determine if the variable is a projected x or y horizontal spatial
+        coordinate based on the `standard_name` metadata attribute being
+        `projection_x_coordinate` or `projection_y_coordinate`, as defined
+        by the CF Conventions (v1.9). Note, geostationary projections have
+        coordinates with `standard_name` metadata attribute values of
+        `projection_x_angular_coordinate` and
+        `projection_y_angular_coordinate`.
 
         """
         return self.attributes.get('standard_name') in [
-            'projection_x_coordinate', 'projection_x_angular_coordinate',
-            'projection_y_coordinate', 'projection_y_angular_coordinate'
+            'projection_x_coordinate',
+            'projection_x_angular_coordinate',
+            'projection_y_coordinate',
+            'projection_y_angular_coordinate',
         ]
 
     def is_temporal(self) -> bool:
-        """ Determine if the variable is a time based on the `units`
-            metadata attribute being 'since' or other similar options
-            as defined in section 4.4 of the CF Conventions (v1.8).
+        """Determine if the variable is a time based on the `units`
+        metadata attribute being 'since' or other similar options
+        as defined in section 4.4 of the CF Conventions (v1.8).
 
         """
         return ' since ' in self.attributes.get('units', '')
 
     def _get_all_cf_references(self) -> Dict[str, Set[str]]:
-        """ Retrieve a dictionary containing all CF-Convention attributes
-            within the variable that have references to other variables in the
-            granule. These variable references will be fully qualified paths.
+        """Retrieve a dictionary containing all CF-Convention attributes
+        within the variable that have references to other variables in the
+        granule. These variable references will be fully qualified paths.
 
         """
-        return {attribute_name: self._get_cf_references(attribute_name)
-                for attribute_name in CF_REFERENCE_ATTRIBUTES
-                if attribute_name in self.attributes}
+        return {
+            attribute_name: self._get_cf_references(attribute_name)
+            for attribute_name in CF_REFERENCE_ATTRIBUTES
+            if attribute_name in self.attributes
+        }
 
     def _get_cf_references(self, attribute_name: str) -> Set[str]:
-        """ Retrieve an attribute from the parsed varaible metadata, correcting
-            for any known artefacts (missing or incorrect references). Then
-            split this string and qualify the individual references.
+        """Retrieve an attribute from the parsed varaible metadata, correcting
+        for any known artefacts (missing or incorrect references). Then
+        split this string and qualify the individual references.
 
         """
         return self._extract_references(self.attributes.get(attribute_name))
 
-    def _get_configured_attribute(self, attribute_name: str,
-                                  raw_attribute_value: Any) -> Any:
-        """ Check the CFConfig instances assocatiated with the collection for
-            any metadata attribute overrides or supplements that should be
-            applied to the attribute value. A metadata supplement is assumed to
-            imply the attribute should be a string value, with the supplement
-            appended to the end of the value from the granule metadata.
+    def _get_configured_attribute(
+        self, attribute_name: str, raw_attribute_value: Any
+    ) -> Any:
+        """Check the CFConfig instances assocatiated with the collection for
+        any metadata attribute overrides or supplements that should be
+        applied to the attribute value. A metadata supplement is assumed to
+        imply the attribute should be a string value, with the supplement
+        appended to the end of the value from the granule metadata.
 
         """
         cf_overrides = self.cf_config['cf_overrides'].get(attribute_name)
         cf_supplements = self.cf_config['cf_supplements'].get(attribute_name)
 
         if cf_overrides is not None:
             attribute_value = cf_overrides
@@ -274,60 +295,62 @@
             attribute_value = f'{attribute_value}, {cf_supplements}'
         elif cf_supplements is not None:
             attribute_value = cf_supplements
 
         return attribute_value
 
     def _extract_references(self, attribute_string: str) -> Set[str]:
-        """ Given a string value of an attribute, which may contain multiple
-            references to dataset, split that string based on either commas,
-            or spaces (or both together). Then if any reference is a relative
-            path, make it absolute.
+        """Given a string value of an attribute, which may contain multiple
+        references to dataset, split that string based on either commas,
+        or spaces (or both together). Then if any reference is a relative
+        path, make it absolute.
 
         """
         if attribute_string is not None:
             raw_references = re.split(r'\s+|,\s*', attribute_string)
             references = set(self._qualify_references(raw_references))
         else:
             references = set()
 
         return references
 
     def _extract_dimensions(self, variable: ET.Element) -> List[str]:
-        """ Find the dimensions for the variable in question. If there are
-            overriding or supplemental dimensions from the CF configuration
-            file, these are used instead of, or in addition to, the raw
-            dimensions from the `.dmr`. All references are converted to
-            absolute paths in the granule. A set of all fully qualified
-            references is returned.
+        """Find the dimensions for the variable in question. If there are
+        overriding or supplemental dimensions from the CF configuration
+        file, these are used instead of, or in addition to, the raw
+        dimensions from the `.dmr`. All references are converted to
+        absolute paths in the granule. A set of all fully qualified
+        references is returned.
 
         """
         overrides = self.cf_config['cf_overrides'].get('dimensions')
         supplements = self.cf_config['cf_supplements'].get('dimensions')
 
         if overrides is not None:
             dimensions = re.split(r'\s+|,\s*', overrides)
         else:
-            dimensions = [dimension
-                          for dimension in self._get_raw_dimensions(variable)
-                          if dimension is not None]
+            dimensions = [
+                dimension
+                for dimension in self._get_raw_dimensions(variable)
+                if dimension is not None
+            ]
 
         if supplements is not None:
             dimensions += re.split(r'\s+|,\s*', supplements)
 
         return self._qualify_references(dimensions)
 
     def _qualify_references(self, raw_references: List[str]) -> List[str]:
-        """ Take a list of local references to other variables, and produce a
-            list of absolute references.
+        """Take a list of local references to other variables, and produce a
+        list of absolute references.
 
-            Trailing colons are removed from variable references. These might
-            occur in some CF-Convention defined formats of the grid_mapping
-            metadata attribute. E.g. "crs: grid_y crs: grid_x" (See section 5.6
-            of CF-Conventions).
+        Trailing colons are removed from variable references. These might
+        occur in some CF-Convention defined formats of the grid_mapping
+        metadata attribute. E.g. "crs: grid_y crs: grid_x" (See section 5.6
+        of CF-Conventions).
 
         """
         references = []
 
         if self.group_path is not None:
             for reference in raw_references:
                 reference = reference.rstrip(':')
@@ -357,113 +380,116 @@
                     absolute_path = f'/{reference}'
 
                 references.append(absolute_path)
 
         return references
 
     def _construct_absolute_path(self, reference: str) -> str:
-        """ For a relative reference to another variable (e.g. '../latitude'),
-            construct an absolute path by combining the reference with the
-            group path of the variable.
+        """For a relative reference to another variable (e.g. '../latitude'),
+        construct an absolute path by combining the reference with the
+        group path of the variable.
 
         """
         relative_prefix = '../'
         group_path_pieces = self.group_path.split('/')
 
         while reference.startswith(relative_prefix):
-            reference = reference[len(relative_prefix):]
+            reference = reference[len(relative_prefix) :]
             group_path_pieces.pop()
 
         absolute_path = group_path_pieces + [reference]
         return '/'.join(absolute_path)
 
     def _extract_group_and_name(self) -> Tuple[str]:
-        """ Extract the group and base name of a variable from the full path,
-            e.g. '/this/is/my/variable' should return a two-element tuple:
-            ('/this/is/my', 'variable').
+        """Extract the group and base name of a variable from the full path,
+        e.g. '/this/is/my/variable' should return a two-element tuple:
+        ('/this/is/my', 'variable').
 
         """
         split_full_path = self.full_name_path.split('/')
         name = split_full_path.pop(-1)
         group_path = '/'.join(split_full_path) or None
 
         return group_path, name
 
 
 class VariableFromDmr(VariableBase):
-    """ This child class inherits from the `VariableBase` class, and implements
-        the abstract methods assuming the variable source is part of an XML
-        element tree.
+    """This child class inherits from the `VariableBase` class, and implements
+    the abstract methods assuming the variable source is part of an XML
+    element tree.
 
     """
+
     def _get_data_type(self, variable: ET.Element) -> str:
-        """ Extract a string representation of the variable data type. """
+        """Extract a string representation of the variable data type."""
         return variable.tag.lstrip(self.namespace).lower()
 
     def _get_shape(self, variable: ET.Element) -> Tuple[int]:
-        """ Extract the shape of the variable data array. This is not yet
-            implemented as the Dimension information is currently unavailable
-            to the Variable XML content.
+        """Extract the shape of the variable data array. This is not yet
+        implemented as the Dimension information is currently unavailable
+        to the Variable XML content.
 
         """
 
     def _get_attributes(self, variable: ET.Element) -> Dict:
-        """ Locate all child Attribute elements of the variable and extract
-            their associated values.
+        """Locate all child Attribute elements of the variable and extract
+        their associated values.
 
         """
         return {
-            attribute.get('name'): self._get_attribute(variable,
-                                                       attribute.get('name'))
+            attribute.get('name'): self._get_attribute(variable, attribute.get('name'))
             for attribute in variable.findall(f'{self.namespace}Attribute')
         }
 
     def _get_attribute(self, variable: ET.Element, attribute_name: str) -> Any:
-        """ Extract the value of an XML Attribute element, casting it to the
-            appropriate type. Apply any necessary metadata overrides or
-            supplements.
+        """Extract the value of an XML Attribute element, casting it to the
+        appropriate type. Apply any necessary metadata overrides or
+        supplements.
 
         """
         raw_value = get_xml_attribute(variable, attribute_name, self.namespace)
         return self._get_configured_attribute(attribute_name, raw_value)
 
     def _get_raw_dimensions(self, variable: ET.Element) -> List[str]:
-        """ Extract the raw dimension names from a <Dim /> XML element. """
-        return [dimension.get('name')
-                for dimension
-                in variable.findall(f'{self.namespace}Dim')]
+        """Extract the raw dimension names from a <Dim /> XML element."""
+        return [
+            dimension.get('name')
+            for dimension in variable.findall(f'{self.namespace}Dim')
+        ]
 
 
 class VariableFromNetCDF4(VariableBase):
-    """ This child class inherits from the `VariableBase` class, and implements
-        the abstract methods assuming the variable source is part of a NetCDF-4
-        file.
+    """This child class inherits from the `VariableBase` class, and implements
+    the abstract methods assuming the variable source is part of a NetCDF-4
+    file.
 
     """
+
     def _get_data_type(self, variable: NetCDF4Variable) -> str:
-        """ Extract a string representation of the variable data type. """
+        """Extract a string representation of the variable data type."""
         return variable.datatype.name
 
     def _get_shape(self, variable: NetCDF4Variable) -> Tuple[int]:
-        """ Extract the shape of the variable data array. """
+        """Extract the shape of the variable data array."""
         return variable.shape
 
     def _get_attributes(self, variable: NetCDF4Variable) -> Dict:
-        """ Identify all variable attributes and save them to a dictionary. """
-        return {attribute_name: self._get_attribute(variable, attribute_name)
-                for attribute_name in variable.ncattrs()}
-
-    def _get_attribute(self, variable: NetCDF4Variable,
-                       attribute_name: str) -> Any:
-        """ Extract the value of the metadata attribute, applying any necessary
-            overrides or supplements.
+        """Identify all variable attributes and save them to a dictionary."""
+        return {
+            attribute_name: self._get_attribute(variable, attribute_name)
+            for attribute_name in variable.ncattrs()
+        }
+
+    def _get_attribute(self, variable: NetCDF4Variable, attribute_name: str) -> Any:
+        """Extract the value of the metadata attribute, applying any necessary
+        overrides or supplements.
 
         """
         raw_value = variable.__dict__.get(attribute_name)
         return self._get_configured_attribute(attribute_name, raw_value)
 
     def _get_raw_dimensions(self, variable: NetCDF4Variable) -> List[str]:
-        """ Retrieve the dimension names as they are stored within the
-            variable.
+        """Retrieve the dimension names as they are stored within the
+        variable.
 
         """
         return list(variable.dimensions)
```

