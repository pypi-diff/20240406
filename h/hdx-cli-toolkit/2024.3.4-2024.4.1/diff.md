# Comparing `tmp/hdx_cli_toolkit-2024.3.4.tar.gz` & `tmp/hdx_cli_toolkit-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx_cli_toolkit-2024.3.4.tar", last modified: Tue Mar 26 16:27:15 2024, max compression
+gzip compressed data, was "hdx_cli_toolkit-2024.4.1.tar", last modified: Sat Apr  6 13:26:23 2024, max compression
```

## Comparing `hdx_cli_toolkit-2024.3.4.tar` & `hdx_cli_toolkit-2024.4.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 16:27:15.005366 hdx_cli_toolkit-2024.3.4/
--rw-rw-rw-   0        0        0     1101 2024-03-26 16:12:26.000000 hdx_cli_toolkit-2024.3.4/LICENSE
--rw-rw-rw-   0        0        0     6621 2024-03-26 16:27:15.001980 hdx_cli_toolkit-2024.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     4716 2024-03-24 13:03:41.000000 hdx_cli_toolkit-2024.3.4/README.md
--rw-rw-rw-   0        0        0     1201 2024-03-26 16:12:26.000000 hdx_cli_toolkit-2024.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-26 16:27:15.005366 hdx_cli_toolkit-2024.3.4/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-11-20 07:15:00.000000 hdx_cli_toolkit-2024.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 16:27:14.853192 hdx_cli_toolkit-2024.3.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-26 16:27:14.897293 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit/
--rw-rw-rw-   0        0        0        0 2024-01-05 08:28:50.000000 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit/__init__.py
--rw-rw-rw-   0        0        0    14145 2024-03-26 16:12:26.000000 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit/cli.py
--rw-rw-rw-   0        0        0    13788 2024-03-24 13:03:41.000000 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit/hdx_utilities.py
--rw-rw-rw-   0        0        0    10025 2024-03-24 13:03:41.000000 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit/utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-26 16:27:14.998037 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit.egg-info/
--rw-rw-rw-   0        0        0     6621 2024-03-26 16:27:14.000000 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2024-03-26 16:27:14.000000 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 16:27:14.000000 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-03-26 16:27:14.000000 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      116 2024-03-26 16:27:14.000000 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-03-26 16:27:14.000000 hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-26 16:27:14.973169 hdx_cli_toolkit-2024.3.4/src/temp/
--rw-rw-rw-   0        0        0     3207 2024-03-24 07:07:45.000000 hdx_cli_toolkit-2024.3.4/src/temp/resource_order_test.py
-drwxrwxrwx   0        0        0        0 2024-03-26 16:27:14.993836 hdx_cli_toolkit-2024.3.4/tests/
--rw-rw-rw-   0        0        0     1926 2024-03-24 13:03:41.000000 hdx_cli_toolkit-2024.3.4/tests/test_cli.py
--rw-rw-rw-   0        0        0     2007 2024-03-24 13:03:41.000000 hdx_cli_toolkit-2024.3.4/tests/test_hdx_utilities.py
--rw-rw-rw-   0        0        0     3887 2024-03-18 06:47:36.000000 hdx_cli_toolkit-2024.3.4/tests/test_integration.py
--rw-rw-rw-   0        0        0     2218 2024-02-22 08:06:55.000000 hdx_cli_toolkit-2024.3.4/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:23.981731 hdx_cli_toolkit-2024.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/hdx_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/tests/test_cli_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/tests/test_hdx_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/tests/test_hdx_utilities_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/tests/test_utilities.py
```

### Comparing `hdx_cli_toolkit-2024.3.4/LICENSE` & `hdx_cli_toolkit-2024.4.1/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2024 Ian Hopkinson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2024 Ian Hopkinson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `hdx_cli_toolkit-2024.3.4/README.md` & `hdx_cli_toolkit-2024.4.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,118 @@
-# HDX CLI Toolkit
-
-## Overview
-
-This toolkit provides a commandline interface to the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) to allow for bulk modification operations and other administrative activities such as getting `id` values for users and organization. It is useful for those managing HDX and developers building data pipelines for HDX. The currently supported commands are as follows:
-
-```
-  configuration              Print configuration information to terminal
-  get_organization_metadata  Get an organization id and other metadata
-  get_user_metadata          Get user id and other metadata
-  list                       List datasets in HDX
-  print                      Print datasets in HDX to the terminal
-  quickcharts                Upload QuickChart JSON description to HDX
-  showcase                   Upload showcase to HDX
-  update                     Update datasets in HDX
-  update_resource            Update a resource in HDX
-```
-
-It is a thin wrapper to the [hdx-python-api](https://github.com/OCHA-DAP/hdx-python-api) library written by Mike Rans.
-
-The library requires some configuration, described below, to authenticate to the HDX instance.
-
-## Installation
-`hdx-cli-toolkit` is a Python application published to the PyPI package repository, therefore it can be installed easily with:
-
-```pip install hdx_cli_toolkit```
-
-Users may prefer to make a global, isolated installation using [pipx](https://pypi.org/project/pipx/) which will make the `hdx-toolkit` commands available across their projects:
-
-```pipx install hdx_cli_toolkit```
-
-`hdx-cli-toolkit` uses the `hdx-python-api` library, this requires the following to be added to a file called `.hdx_configuration.yaml` in the user's home directory.
-
-```
-hdx_key_stage: "[hdx_key from the staging HDX site]"
-hdx_key: "[hdx_key from the prod HDX site]"
-```
-
-A user agent (`hdx_cli_toolkit_*`) is specified in the `~/.useragents.yaml` file with the * replaced with the users initials.
-```
-hdx-cli-toolkit:
-    preprefix: [YOUR_ORGANIZATION]
-    user_agent: hdx_cli_toolkit_ih
-```
-
-## Usage
-
-The `hdx-toolkit` is built using the Python `click` library. Details of the currently implemented commands can be revealed by running `hdx-toolkit --help`:
-
-```
-$ hdx-toolkit --help
-Usage: hdx-toolkit [OPTIONS] COMMAND [ARGS]...
-
-  Tools for Commandline interactions with HDX
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  configuration              Print configuration information to terminal
-  get_organization_metadata  Get an organization id and other metadata
-  get_user_metadata          Get user id and other metadata
-  list                       List datasets in HDX
-  print                      Print datasets in HDX to the terminal
-  quickcharts                Upload QuickChart JSON description to HDX
-  showcase                   Upload showcase to HDX
-  update                     Update datasets in HDX
-  update_resource            Update a resource in HDX
-```
-
-And details of the arguments for a command can be found using:
-
-```shell
-hdx-toolkit [COMMAND] --help
-```
-
-A detailed walk through of commands can be found in the [DEMO.md](DEMO.md) file
-
-## Contributions
-
-For developers the code should be cloned installed from the [GitHub repo](https://github.com/OCHA-DAP/hdx-cli-toolkit), and a virtual enviroment created:
-
-```shell
-python -m venv venv
-source venv/Scripts/activate
-```
-
-And then an editable installation created:
-
-```shell
-pip install -e .
-```
-
-The library is then configured, as described above.
-
-This project uses a GitHub Action to run tests and linting. It requires the following environment variables/secrets to be set in the `test` environment:
-
-```
-HDX_KEY - secret. Value: fake secret
-HDX_KEY_STAGE - secret. Value: a live API key for the stage server
-HDX_SITE - environment variable. Value: stage
-USER_AGENT - environment variable. Value: hdx_cli_toolkit_gha
-PREPREFIX - - environment variable. Value: [YOUR_organization]
-```
-
-Most tests use mocking in place of HDX, although the `test_integration.py` suite runs against the `stage` server.
-
-New features should be developed against a GitHub issue on a separate branch with a name starting `GH[issue number]_`. `PULL_REQUEST_TEMPLATE.md` should be used in preparing pull requests. Versioning is updated manually in `pyproject.toml` and is described in the template, in brief it is CalVer `YYYY.MM.Micro`.
-
-## Publication
-
-Publication to PyPI is done using `hatch` which requires the following environment variables:
-
-```
-HATCH_INDEX_USER - set to `__token__`
-HATCH_INDEX_AUTH - API key provided by PyPI
-```
+# HDX CLI Toolkit
+
+## Overview
+
+This toolkit provides a commandline interface to the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) to allow for bulk modification operations and other administrative activities such as getting `id` values for users and organization. It is useful for those managing HDX and developers building data pipelines for HDX. The currently supported commands are as follows:
+
+```
+  configuration              Print configuration information to terminal
+  get_organization_metadata  Get an organization id and other metadata
+  get_user_metadata          Get user id and other metadata
+  list                       List datasets in HDX
+  print                      Print datasets in HDX to the terminal
+  quickcharts                Upload QuickChart JSON description to HDX
+  showcase                   Upload showcase to HDX
+  update                     Update datasets in HDX
+  update_resource            Update a resource in HDX
+```
+
+It is a thin wrapper to the [hdx-python-api](https://github.com/OCHA-DAP/hdx-python-api) library written by Mike Rans.
+
+The library requires some configuration, described below, to authenticate to the HDX instance.
+
+## Installation
+`hdx-cli-toolkit` is a Python application published to the PyPI package repository, therefore it can be installed easily with:
+
+```pip install hdx_cli_toolkit```
+
+Users may prefer to make a global, isolated installation using [pipx](https://pypi.org/project/pipx/) which will make the `hdx-toolkit` commands available across their projects:
+
+```pipx install hdx_cli_toolkit```
+
+`hdx-cli-toolkit` uses the `hdx-python-api` library, this requires the following to be added to a file called `.hdx_configuration.yaml` in the user's home directory.
+
+```
+hdx_key_stage: "[hdx_key from the staging HDX site]"
+hdx_key: "[hdx_key from the prod HDX site]"
+```
+
+A user agent (`hdx_cli_toolkit_*`) is specified in the `~/.useragents.yaml` file with the * replaced with the users initials.
+```
+hdx-cli-toolkit:
+    preprefix: [YOUR_ORGANIZATION]
+    user_agent: hdx_cli_toolkit_ih
+```
+
+## Usage
+
+The `hdx-toolkit` is built using the Python `click` library. Details of the currently implemented commands can be revealed by running `hdx-toolkit --help`:
+
+```
+$ hdx-toolkit --help
+Usage: hdx-toolkit [OPTIONS] COMMAND [ARGS]...
+
+  Tools for Commandline interactions with HDX
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  configuration              Print configuration information to terminal
+  download                   Download dataset resources from HDX
+  get_organization_metadata  Get an organization id and other metadata
+  get_user_metadata          Get user id and other metadata
+  list                       List datasets in HDX
+  print                      Print datasets in HDX to the terminal
+  quickcharts                Upload QuickChart JSON description to HDX
+  showcase                   Upload showcase to HDX
+  update                     Update datasets in HDX
+  update_resource            Update a resource in HDX
+```
+
+And details of the arguments for a command can be found using:
+
+```shell
+hdx-toolkit [COMMAND] --help
+```
+
+A detailed walk through of commands can be found in the [DEMO.md](DEMO.md) file
+
+## Contributions
+
+For developers the code should be cloned installed from the [GitHub repo](https://github.com/OCHA-DAP/hdx-cli-toolkit), and a virtual enviroment created:
+
+```shell
+python -m venv venv
+source venv/Scripts/activate
+```
+
+And then an editable installation created:
+
+```shell
+pip install -e .
+```
+
+The library is then configured, as described above.
+
+This project uses a GitHub Action to run tests and linting. It requires the following environment variables/secrets to be set in the `test` environment:
+
+```
+HDX_KEY - secret. Value: fake secret
+HDX_KEY_STAGE - secret. Value: a live API key for the stage server
+HDX_SITE - environment variable. Value: stage
+USER_AGENT - environment variable. Value: hdx_cli_toolkit_gha
+PREPREFIX - - environment variable. Value: [YOUR_organization]
+```
+
+Most tests use mocking in place of HDX, although the `test_integration.py` suite runs against the `stage` server.
+
+New features should be developed against a GitHub issue on a separate branch with a name starting `GH[issue number]_`. `PULL_REQUEST_TEMPLATE.md` should be used in preparing pull requests. Versioning is updated manually in `pyproject.toml` and is described in the template, in brief it is CalVer `YYYY.MM.Micro`.
+
+## Publication
+
+Publication to PyPI is done using `hatch` which requires the following environment variables:
+
+```
+HATCH_INDEX_USER - set to `__token__`
+HATCH_INDEX_AUTH - API key provided by PyPI
+```
```

### Comparing `hdx_cli_toolkit-2024.3.4/pyproject.toml` & `hdx_cli_toolkit-2024.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-[project]
-name = "hdx_cli_toolkit"
-version = "2024.3.4"
-description = "HDX CLI tool kit for commandline interaction with HDX"
-readme = {file = "README.md", content-type = "text/markdown"}
-license = {file = "LICENSE"}
-requires-python = ">=3.11"
-authors = [
-  {email = "ian.hopkinson@un.org"},
-  {name = "Ian Hopkinson"}
-]
-
-dependencies = [
-  "hdx-python-api",
-  "hdx-python-country",
-  "quantulum3[classifier]", # This stops the UserWarning but has a number of large dependencies
-  "click",
-  "hatch",
-  "pytest",
-  "pytest-cov",
-  "black==23.10.0",
-  "flake8",
-  "pylint"
-]
-
-[project.scripts]
-hdx-toolkit = "hdx_cli_toolkit.cli:hdx_toolkit"
-
-[project.urls]
-repository = "https://github.com/OCHA-DAP/hdx-cli-toolkit"
-
-[build-system]
-requires = ["setuptools >= 61.0.0"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[tool.black]
-line-length = 100
-target-version = ['py311']
-include = '\.pyi?$'
-extend-exclude = '''
-# A regex preceded with ^/ will apply only to files and directories
-# in the root of the project.
-^/foo.py  # exclude a file named foo.py in the root of the project (in addition to the defaults)
+[project]
+name = "hdx_cli_toolkit"
+version = "2024.4.1"
+description = "HDX CLI tool kit for commandline interaction with HDX"
+readme = {file = "README.md", content-type = "text/markdown"}
+license = {file = "LICENSE"}
+requires-python = ">=3.11"
+authors = [
+  {email = "ian.hopkinson@un.org"},
+  {name = "Ian Hopkinson"}
+]
+
+dependencies = [
+  "hdx-python-api",
+  "hdx-python-country",
+  "quantulum3[classifier]", # This stops the UserWarning but has a number of large dependencies
+  "click",
+  "hatch",
+  "pytest",
+  "pytest-cov",
+  "black==23.10.0",
+  "flake8",
+  "pylint"
+]
+
+[project.scripts]
+hdx-toolkit = "hdx_cli_toolkit.cli:hdx_toolkit"
+
+[project.urls]
+repository = "https://github.com/OCHA-DAP/hdx-cli-toolkit"
+
+[build-system]
+requires = ["setuptools >= 61.0.0"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.black]
+line-length = 100
+target-version = ['py311']
+include = '\.pyi?$'
+extend-exclude = '''
+# A regex preceded with ^/ will apply only to files and directories
+# in the root of the project.
+^/foo.py  # exclude a file named foo.py in the root of the project (in addition to the defaults)
 '''
```

### Comparing `hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit/cli.py` & `hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/hdx_utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,488 +1,395 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
-import json
-import os
-import time
-
-from collections.abc import Callable
-
-import click
-from click.decorators import FC
-
-from hdx.api.configuration import ConfigurationError
-from hdx.utilities.path import script_dir_plus_file
-
-from hdx_cli_toolkit.utilities import (
-    write_dictionary,
-    print_table_from_list_of_dicts,
-    censor_secret,
-    make_conversion_func,
-    print_banner,
-)
-
-from hdx_cli_toolkit.hdx_utilities import (
-    add_showcase,
-    add_quickcharts,
-    get_organizations_from_hdx,
-    get_users_from_hdx,
-    update_values_in_hdx,
-    configure_hdx_connection,
-    update_resource_in_hdx,
-    get_filtered_datasets,
-    decorate_dataset_with_extras,
-)
-
-
-@click.group()
-def hdx_toolkit() -> None:
-    """Tools for Commandline interactions with HDX"""
-
-
-OPTIONS = [
-    click.option(
-        "--organization",
-        is_flag=False,
-        default="",
-        help="an organization name",
-    ),
-    click.option(
-        "--key",
-        is_flag=False,
-        default="private",
-        help="a single key to list alongside organization",
-    ),
-    click.option(
-        "--value",
-        is_flag=False,
-        default=None,
-        help="a value to set",
-    ),
-    click.option(
-        "--dataset_filter",
-        is_flag=False,
-        default="*",
-        help="a dataset name or pattern on which to filter list",
-    ),
-    click.option(
-        "--query",
-        is_flag=False,
-        default=None,
-        help=(
-            "a dataset query string to pass to CKAN, "
-            "organization and dataset_filter are ignored if it is provided"
-        ),
-    ),
-    click.option(
-        "--hdx_site",
-        is_flag=False,
-        default="stage",
-        help="an hdx_site value {stage|prod}",
-    ),
-]
-
-
-def multi_decorator(options: list[Callable[[FC], FC]]) -> Callable[[FC], FC]:
-    def decorator(f: FC) -> FC:
-        for option in reversed(options):
-            f = option(f)
-
-        return f
-
-    return decorator
-
-
-@hdx_toolkit.command(name="list")
-@multi_decorator(OPTIONS)
-@click.option(
-    "--output_path",
-    is_flag=False,
-    default=None,
-    help="A file path to export data from list to CSV",
-)
-def list_datasets(
-    organization: str = "",
-    key: str = "private",
-    value: str = "value",
-    dataset_filter: str = "*",
-    query: str = None,
-    hdx_site: str = "stage",
-    output_path: str = None,
-):
-    """List datasets in HDX"""
-    print_banner("list")
-
-    filtered_datasets = get_filtered_datasets(
-        organization=organization,
-        dataset_filter=dataset_filter,
-        query=query,
-        hdx_site=hdx_site,
-    )
-
-    keys = key.split(",")
-    output_template = {"dataset_name": ""}
-    for key_ in keys:
-        output_template[key_] = ""
-
-    output = []
-    for dataset in filtered_datasets:
-        output_row = output_template.copy()
-        output_row["dataset_name"] = dataset["name"]
-        for key_ in keys:
-            output_row[key_] = dataset.get(key_, "")
-        output.append(output_row)
-
-    print_table_from_list_of_dicts(output)
-    if output_path is not None:
-        status = write_dictionary(output_path, output, append=False)
-        print(status, flush=True)
-
-
-@hdx_toolkit.command(name="update")
-@multi_decorator(OPTIONS)
-def update(
-    organization: str = "",
-    key: str = "private",
-    value: str = "value",
-    dataset_filter: str = "*",
-    query: str = None,
-    hdx_site: str = "stage",
-):
-    """Update datasets in HDX"""
-    print_banner("Update")
-    filtered_datasets = get_filtered_datasets(
-        organization=organization,
-        dataset_filter=dataset_filter,
-        query=query,
-        hdx_site=hdx_site,
-    )
-
-    if len(filtered_datasets) == 0:
-        print("Specified filter returns no datasets", flush=True)
-        return
-
-    print(f"Updating key '{key}' with value '{value}'")
-    conversion_func, type_name = make_conversion_func(filtered_datasets[0][key])
-    if conversion_func is None:
-        print(f"Type name '{type_name}' is not recognised, aborting", flush=True)
-        return
-
-    print(f"Detected value type is '{type_name}'", flush=True)
-    print(
-        f"{'dataset_name':<70.70}{'old value':<20.20}{'new value':<20.20}"
-        f"{'Time to update/seconds':<25.25}",
-        flush=True,
-    )
-    n_changed, n_failures = update_values_in_hdx(
-        filtered_datasets, key, value, conversion_func, hdx_site=hdx_site
-    )
-
-    print(f"Changed {n_changed} values", flush=True)
-    print(f"{n_failures} failures as evidenced by HDXError", flush=True)
-
-
-@hdx_toolkit.command(name="print")
-@multi_decorator(OPTIONS)
-@click.option(
-    "--with_extras",
-    is_flag=True,
-    default=False,
-    help=(
-        "If set resources, resource_views (QuickCharts) "
-        "and Showcases are added to the dataset output"
-    ),
-)
-def print_datasets(
-    organization: str = "healthsites",
-    key: str = "private",
-    value: str = "value",
-    dataset_filter: str = "*",
-    query: str = None,
-    hdx_site: str = "stage",
-    with_extras: bool = False,
-):
-    """Print datasets in HDX to the terminal"""
-
-    filtered_datasets = get_filtered_datasets(
-        organization=organization,
-        dataset_filter=dataset_filter,
-        hdx_site=hdx_site,
-        query=query,
-        verbose=False,
-    )
-
-    print("[", flush=True)
-    for i, dataset in enumerate(filtered_datasets):
-        output_dict = dataset.data
-        if with_extras:
-            output_dict = decorate_dataset_with_extras(dataset)
-
-        print(json.dumps(output_dict, indent=4), flush=True)
-        if i != len(filtered_datasets) - 1:
-            print(",", flush=True)
-    print("]", flush=True)
-
-
-@hdx_toolkit.command(name="get_organization_metadata")
-@click.option(
-    "--organization",
-    is_flag=False,
-    default="",
-    help="an organization name, wildcards are implicitly included",
-)
-@click.option(
-    "--hdx_site",
-    is_flag=False,
-    default="stage",
-    help="an hdx_site value {stage|prod}",
-)
-@click.option(
-    "--verbose",
-    is_flag=True,
-    default=False,
-    help="if true show all organization metadata",
-)
-def get_organization_metadata(organization: str, hdx_site: str = "stage", verbose: bool = False):
-    """Get an organization id and other metadata"""
-    print_banner("Get organization Metadata")
-    configure_hdx_connection(hdx_site=hdx_site)
-
-    filtered_organizations = get_organizations_from_hdx(organization, hdx_site=hdx_site)
-    for filtered_organization in filtered_organizations:
-        if verbose:
-            print(json.dumps(filtered_organization.data, indent=2), flush=True)
-        else:
-            print(
-                f"{filtered_organization['name']:<50.50}: {filtered_organization['id']}",
-                flush=True,
-            )
-
-
-@hdx_toolkit.command(name="get_user_metadata")
-@click.option(
-    "--user",
-    is_flag=False,
-    default="",
-    help="a user name or email, wildcards are implicitly included",
-)
-@click.option(
-    "--hdx_site",
-    is_flag=False,
-    default="stage",
-    help="an hdx_site value {stage|prod}",
-)
-@click.option(
-    "--verbose",
-    is_flag=True,
-    default=False,
-    help="if true show all user metadata",
-)
-def get_user_metadata(user: str, hdx_site: str = "stage", verbose: bool = False):
-    """Get user id and other metadata"""
-    print_banner("Get User Metadata")
-
-    user_list = get_users_from_hdx(user, hdx_site=hdx_site)
-    for a_user in user_list:
-        if verbose:
-            print(json.dumps(a_user.data, indent=2), flush=True)
-        else:
-            print(
-                f"{a_user['name']:<50.50}: {a_user['id']}",
-                flush=True,
-            )
-
-
-@hdx_toolkit.command(name="configuration")
-def show_configuration():
-    """Print configuration information to terminal"""
-    print_banner("configuration")
-    # Check files
-    user_hdx_config_yaml = os.path.join(os.path.expanduser("~"), ".hdx_configuration.yaml")
-    default_hdx_config_yaml = script_dir_plus_file(
-        "hdx_base_configuration.yaml", ConfigurationError
-    )
-
-    if os.path.exists(user_hdx_config_yaml):
-        click.secho(
-            f"Found a user configuration file at {user_hdx_config_yaml}. "
-            "Contents (secrets censored):",
-            bold=True,
-        )
-        with open(user_hdx_config_yaml, encoding="utf-8") as config_file:
-            config_file_contents = config_file.read()
-            rows = config_file_contents.split("\n")
-            for row in rows:
-                if row.startswith("hdx_key"):
-                    key_part, secret_part = row.split(":")
-                    secret_part = censor_secret(secret_part)
-                    row = key_part + ': "' + secret_part
-                print(row, flush=True)
-
-    user_agent_config_yaml = os.path.join(os.path.expanduser("~"), ".useragents.yaml")
-    if os.path.exists(user_agent_config_yaml):
-        click.secho(f"User agents file found at {user_agent_config_yaml}", bold=True)
-        with open(user_agent_config_yaml, encoding="utf-8") as config_file:
-            user_agents_file_contents = config_file.read()
-            print(user_agents_file_contents, flush=True)
-
-    # Check Environment variables
-    environment_variables = ["HDX_KEY", "HDX_KEY_STAGE", "HDX_SITE", "HDX_URL"]
-    click.secho(
-        "Values of relevant environment variables (used in absence of supplied values):", bold=True
-    )
-    for variable in environment_variables:
-        env_variable = os.getenv(variable)
-        if env_variable is not None:
-            if "HDX_KEY" in variable:
-                env_variable = censor_secret(env_variable)
-            print(f"{variable}:{env_variable}", flush=True)
-        else:
-            print(f"{variable} is not set", flush=True)
-
-    click.secho(
-        f"\nDefault base configuration file is at {default_hdx_config_yaml}. Contents:", bold=True
-    )
-    with open(default_hdx_config_yaml, encoding="utf-8") as config_file:
-        config_file_contents = config_file.read()
-        print(config_file_contents, flush=True)
-
-
-@hdx_toolkit.command(name="quickcharts")
-@click.option(
-    "--dataset_filter",
-    is_flag=False,
-    default="*",
-    help="a dataset name",
-)
-@click.option(
-    "--hdx_site",
-    is_flag=False,
-    default="stage",
-    help="an hdx_site value {stage|prod}",
-)
-@click.option(
-    "--resource_name",
-    is_flag=False,
-    default="stage",
-    help="name of resource to which the QuickCharts are attached",
-)
-@click.option(
-    "--hdx_hxl_preview_file_path",
-    is_flag=False,
-    default="stage",
-    help="name of resource to which the QuickCharts are attached",
-)
-def quickcharts(
-    dataset_filter: str = "",
-    hdx_site: str = "stage",
-    resource_name: str = "",
-    hdx_hxl_preview_file_path: str = "",
-):
-    """Upload QuickChart JSON description to HDX"""
-    print_banner("quickcharts")
-    print(
-        f"Adding Quick Chart defined at '{hdx_hxl_preview_file_path}' to dataset "
-        f"'{dataset_filter}', resource '{resource_name}'"
-    )
-    t0 = time.time()
-    status = add_quickcharts(dataset_filter, hdx_site, resource_name, hdx_hxl_preview_file_path)
-
-    print(status, flush=True)
-
-    print(f"Quick Chart update took {time.time() - t0:.2f} seconds")
-
-
-@hdx_toolkit.command(name="showcase")
-@click.option(
-    "--showcase_name",
-    is_flag=False,
-    default="*",
-    help="showcase name",
-)
-@click.option(
-    "--hdx_site",
-    is_flag=False,
-    default="stage",
-    help="an hdx_site value {stage|prod}",
-)
-@click.option(
-    "--attributes_file_path",
-    is_flag=False,
-    default="stage",
-    help="path to the attributes file describing the showcase",
-)
-def showcase(
-    showcase_name: str = "",
-    hdx_site: str = "stage",
-    attributes_file_path: str = "",
-):
-    """Upload showcase to HDX"""
-    print_banner("showcase")
-    print(f"Adding showcase defined at '{attributes_file_path}'")
-    t0 = time.time()
-    statuses = add_showcase(showcase_name, hdx_site, attributes_file_path)
-    for status in statuses:
-        print(status, flush=True)
-
-    print(f"Showcase update took {time.time() - t0:.2f} seconds")
-
-
-@hdx_toolkit.command(name="update_resource")
-@click.option(
-    "--dataset_name",
-    is_flag=False,
-    default="*",
-    help="name of the dataset to update",
-)
-@click.option(
-    "--resource_name",
-    is_flag=False,
-    default="*",
-    help="name of the resource in the dataset to update",
-)
-@click.option(
-    "--hdx_site",
-    is_flag=False,
-    default="stage",
-    help="an hdx_site value {stage|prod}",
-)
-@click.option(
-    "--resource_file_path",
-    is_flag=False,
-    default="stage",
-    help="path to the resource file to upload",
-)
-@click.option(
-    "--live",
-    is_flag=True,
-    default=False,
-    help="if present then update to HDX is made, if absent then a dry run is done",
-)
-@click.option(
-    "--description",
-    is_flag=False,
-    default="new resource",
-    help="if the resource is to be added, rather than updated this provides the description",
-)
-def update_resource(
-    dataset_name: str = "",
-    resource_name: str = "",
-    hdx_site: str = "stage",
-    resource_file_path: str = "",
-    live: bool = False,
-    description: str = "new resource",
-):
-    """Update a resource in HDX"""
-    print_banner("Update resource")
-    print(
-        f"Updating/adding '{resource_name}' in '{dataset_name}' "
-        f"with file at '{resource_file_path}'"
-    )
-    t0 = time.time()
-    statuses = update_resource_in_hdx(
-        dataset_name, resource_name, hdx_site, resource_file_path, live, description=description
-    )
-    for status in statuses:
-        print(status, flush=True)
-
-    print(f"Resource update took {time.time() - t0:.2f} seconds")
+#!/usr/bin/env python
+# encoding: utf-8
+
+
+import fnmatch
+import json
+import os
+import time
+import traceback
+
+from pathlib import Path
+
+import yaml
+
+from hdx.api.configuration import Configuration, ConfigurationError
+from hdx.data.organization import Organization
+from hdx.data.resource_view import ResourceView
+from hdx.data.hdxobject import HDXError
+from hdx.data.dataset import Dataset
+from hdx.data.showcase import Showcase
+from hdx.data.resource import Resource
+from hdx.data.user import User
+
+from hdx_cli_toolkit.utilities import read_attributes
+
+
+def get_filtered_datasets(
+    organization: str = "",
+    dataset_filter: str = "*",
+    query: str = None,
+    hdx_site: str = "stage",
+    verbose: bool = True,
+) -> list[Dataset]:
+    """A function to return a list of datasets selected by some selection criteria based on
+    organization, dataset name, or CKAN query strings. The verbose flag is provided so
+    summary output can be suppressed for output to file in the print command.
+
+    Keyword Arguments:
+        organization {str} -- an organization name (default: {""})
+        key {str} -- _description_ (default: {"private"})
+        value {str} -- _description_ (default: {"value"})
+        dataset_filter {str} -- a filter for dataset name, can contain wildcards (default: {"*"})
+        query {str} -- a query string to use in the CKAN search API (default: {None})
+        hdx_site {str} -- target HDX site {prod|stage} (default: {"stage"})
+        verbose {bool} -- if True prints summary information (default: {True})
+
+    Returns:
+        list[Dataset] -- a list of datasets satisfying the selection criteria
+    """
+    configure_hdx_connection(hdx_site=hdx_site, verbose=False)
+
+    if organization != "":
+        organization = Organization.read_from_hdx(organization)
+        datasets = organization.get_datasets(include_private=True)
+    elif query is not None:
+        datasets = Dataset.search_in_hdx(query=query)
+        organization = {"display_name": "", "name": ""}
+    else:
+        dataset = Dataset.read_from_hdx(dataset_filter)
+        if dataset is None:
+            datasets = []
+            organization = {"display_name": "", "name": ""}
+        else:
+            datasets = [dataset]
+            organization = dataset.get_organization()
+            organization = {"display_name": organization["title"], "name": organization["name"]}
+
+    filtered_datasets = []
+    for dataset in datasets:
+        if fnmatch.fnmatch(dataset["name"], dataset_filter):
+            filtered_datasets.append(dataset)
+
+    if verbose:
+        print(Configuration.read().hdx_site, flush=True)
+        print(
+            f"Found {len(filtered_datasets)} datasets for organization "
+            f"'{organization['display_name']} "
+            f"({organization['name']})' matching filter conditions:",
+            flush=True,
+        )
+
+    return filtered_datasets
+
+
+def update_values_in_hdx(
+    filtered_datasets: list[Dataset], key, value, conversion_func, hdx_site: str = "stage"
+):
+    n_changed = 0
+    n_failures = 0
+    for dataset in filtered_datasets:
+        t0 = time.time()
+        old_value = str(dataset[key])
+        dataset[key] = conversion_func(value)
+        if old_value != str(dataset[key]):
+            n_changed += 1
+        else:
+            print(
+                f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20}"
+                f"{'No update required':<25.25}",
+                flush=True,
+            )
+            continue
+        try:
+            dataset.update_in_hdx(
+                update_resources=False,
+                hxl_update=False,
+                operation="patch",
+                batch_mode="KEEP_OLD",
+                skip_validation=True,
+                ignore_check=True,
+            )
+            print(
+                f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20}"
+                f"{time.time()-t0:0.2f}",
+                flush=True,
+            )
+        except (HDXError, KeyError):
+            if "Authorization Error" in traceback.format_exc():
+                print(
+                    f"Could not update {dataset['name']} on '{hdx_site}' "
+                    "because of an Authorization Error",
+                    flush=True,
+                )
+            else:
+                print(f"Could not update {dataset['name']} on '{hdx_site}'", flush=True)
+            n_failures += 1
+
+            print(
+                f"{dataset['name']:<70.70}{old_value:<20.20}{old_value:<20.20}"
+                f"{time.time()-t0:0.2f}",
+                flush=True,
+            )
+
+    return n_changed, n_failures
+
+
+def get_organizations_from_hdx(organization: str, hdx_site: str = "stage"):
+    configure_hdx_connection(hdx_site)
+    filtered_organizations = []
+    all_organizations = Organization.get_all_organization_names(include_extras=True)
+    for an_organization in all_organizations:
+        if fnmatch.fnmatch(an_organization, f"*{organization}*"):
+            organization_metadata = Organization.read_from_hdx(an_organization)
+            filtered_organizations.append(organization_metadata)
+
+    return filtered_organizations
+
+
+def get_users_from_hdx(user: str, hdx_site: str = "stage"):
+    configure_hdx_connection(hdx_site=hdx_site)
+
+    user_list = User.get_all_users(q=user)
+
+    return user_list
+
+
+def decorate_dataset_with_extras(
+    dataset: Dataset, hdx_site: str = "stage", verbose: bool = False
+) -> dict:
+    """A function to add resource, quickcharts (resource_view) and showcases keys to a dataset
+    dictionary representation for the print command. fs_check_info and hxl_preview_config are
+    converted from JSON objects serialised as single strings to dictionaries to make printed output
+    more readable. This decoration means that the dataset dictionary cannot be uploaded to HDX.
+
+    Arguments:
+        dataset {Dataset} -- a Dataset object to process
+
+    Returns:
+        dict -- a dictionary containing the dataset metadata
+    """
+    configure_hdx_connection(hdx_site, verbose=verbose)
+    output_dict = dataset.data
+    resources = dataset.get_resources()
+    output_dict["resources"] = []
+    for resource in resources:
+        resource_dict = resource.data
+        if "fs_check_info" in resource_dict:
+            resource_dict["fs_check_info"] = json.loads(resource_dict["fs_check_info"])
+        dataset_quickcharts = ResourceView.get_all_for_resource(resource_dict["id"])
+        resource_dict["quickcharts"] = []
+        if dataset_quickcharts is not None:
+            for quickchart in dataset_quickcharts:
+                quickchart_dict = quickchart.data
+                if "hxl_preview_config" in quickchart_dict:
+                    quickchart_dict["hxl_preview_config"] = json.loads(
+                        quickchart_dict["hxl_preview_config"]
+                    )
+                resource_dict["quickcharts"].append(quickchart_dict)
+        output_dict["resources"].append(resource_dict)
+
+    showcases = dataset.get_showcases()
+    output_dict["showcases"] = [x.data for x in showcases]
+
+    return output_dict
+
+
+def add_showcase(showcase_name: str, hdx_site: str, attributes_file_path: str) -> list[str]:
+    configure_hdx_connection(hdx_site)
+    statuses = []
+    showcase_attributes = read_attributes(showcase_name, attributes_filepath=attributes_file_path)
+    showcase = Showcase(
+        {
+            "name": showcase_attributes["name"],
+            "title": showcase_attributes["title"],
+            "notes": showcase_attributes["notes"],
+            "url": showcase_attributes["url"],
+            "image_url": showcase_attributes["image_url"],
+        }
+    )
+    added_tags, unadded_tags = showcase.add_tags(showcase_attributes["tags"])
+    statuses.append(f"{len(added_tags)} of {len(showcase_attributes['tags'])} showcase tags added")
+    if len(unadded_tags) != 0:
+        statuses.append(f"Rejected showcase tags: {unadded_tags}")
+
+    showcase.create_in_hdx()
+    dataset = Dataset.read_from_hdx(showcase_attributes["parent_dataset"])
+    showcase.add_dataset(dataset)
+    statuses.append(f"Added dataset '{dataset['name']}' to showcase '{showcase_name}'")
+
+    return statuses
+
+
+def update_resource_in_hdx(
+    dataset_name: str,
+    resource_name: str,
+    hdx_site: str,
+    resource_file_path: str,
+    live: bool,
+    description: str = "new resource",
+):
+    configure_hdx_connection(hdx_site)
+    statuses = []
+    dataset = Dataset.read_from_hdx(dataset_name)
+    # Check we found a dataset
+    if dataset is None:
+        statuses.append(f"No dataset with the name '{dataset_name}' found on HDX site '{hdx_site}'")
+        return statuses
+
+    statuses.append(f"Found dataset with the name '{dataset_name}' on HDX site '{hdx_site}'")
+    # Check we found a resource
+    resources = dataset.get_resources()
+    resource_to_update = None
+    for resource in resources:
+        if resource["name"] == resource_name:
+            resource_to_update = resource
+
+    # Report on the characteristics of the selected file for upload cf the original if available
+    if not os.path.exists(resource_file_path):
+        statuses.append(f"No file found at file path '{resource_file_path}'")
+        return statuses
+
+    statuses.append(f"Found file to upload at '{resource_file_path}'")
+
+    if resource_to_update is not None:
+        url = resource_to_update["url"]
+        original_filename = url[(url.rfind("/") + 1) :]  # noqa: E203
+        original_size = resource_to_update["size"]
+        statuses.append(
+            f"Original resource filename '{original_filename}' with size {original_size}"
+        )
+
+    replacement_filename = os.path.basename(resource_file_path)
+    file_stats = os.stat(resource_file_path)
+    replacement_size = file_stats.st_size
+    statuses.append(
+        f"Replacement resource filename '{replacement_filename}' with size {replacement_size}"
+    )
+
+    # This is the "add resource branch"
+    if resource_to_update is None:
+        statuses.append(
+            f"No resource with the name '{resource_name}' found on dataset '{dataset_name}', "
+            "adding file as new resource."
+        )
+        # Make a new resource
+        new_resource = Resource(
+            {
+                "name": resource_name,
+                "description": description,
+            }
+        )
+
+        new_resource.set_file_to_upload(resource_file_path, guess_format_from_suffix=True)
+        resource_list = [new_resource]
+        resource_list.extend(resources)
+        dataset.add_update_resources(resource_list, ignore_datasetid=True)
+        if live:
+            # It seems this match_resource_order keyword is not respected
+            dataset.update_in_hdx(match_resource_order=True)
+            # So we reload the dataset from HDX and force a reorder
+            revised_dataset = Dataset.read_from_hdx(dataset_name)
+            resources_check = revised_dataset.get_resources()
+
+            reordered_resource_ids = [
+                x["id"] for x in resources_check if x["name"] == resource_name
+            ]
+            reordered_resource_ids.extend(
+                [x["id"] for x in resources_check if x["name"] != resource_name]
+            )
+
+            revised_dataset.reorder_resources(resource_ids=reordered_resource_ids)
+            statuses.append("Addition to HDX successful")
+            return statuses
+    else:
+        resource_to_update.set_file_to_upload(resource_file_path, guess_format_from_suffix=True)
+        if live:
+            resource_to_update.update_in_hdx()
+            statuses.append("Update to HDX successful")
+            return statuses
+
+    statuses.append("No '--live' flag supplied so no update to HDX made, otherwise successful")
+    return statuses
+
+
+def add_quickcharts(dataset_name, hdx_site, resource_name, hdx_hxl_preview_file_path):
+    configure_hdx_connection(hdx_site=hdx_site)
+    status = "Successful"
+
+    # read the json file
+    with open(hdx_hxl_preview_file_path, "r", encoding="utf-8") as json_file:
+        recipe = json.load(json_file)
+    # extract appropriate keys
+    processed_recipe = {
+        "description": "",
+        "title": "Quick Charts",
+        "view_type": "hdx_hxl_preview",
+        "hxl_preview_config": "",
+    }
+
+    # convert the configuration to a string
+    stringified_config = json.dumps(
+        recipe["hxl_preview_config"], indent=None, separators=(",", ":")
+    )
+    processed_recipe["hxl_preview_config"] = stringified_config
+    # write out yaml to a temp file
+    temp_yaml_path = f"{hdx_hxl_preview_file_path}.temp.yaml"
+    with open(temp_yaml_path, "w", encoding="utf-8") as yaml_file:
+        yaml.dump(processed_recipe, yaml_file)
+
+    dataset = Dataset.read_from_hdx(dataset_name)
+    dataset.generate_quickcharts(resource=resource_name, path=temp_yaml_path)
+    dataset.update_in_hdx(update_resources=False, hxl_update=False)
+
+    # delete the temp file
+    if os.path.exists(temp_yaml_path):
+        os.remove(temp_yaml_path)
+
+    return status
+
+
+def download_hdx_datasets(
+    dataset_filter: str,
+    resource_filter: str = "*",
+    hdx_site: str = "stage",
+    download_directory: str = None,
+):
+    configure_hdx_connection(hdx_site=hdx_site)
+    if download_directory is None:
+        download_directory = os.path.join(os.path.dirname(__file__), "output")
+
+    Path(download_directory).mkdir(parents=True, exist_ok=True)
+
+    if resource_filter is None:
+        resource_filter = "*"
+
+    dataset = Dataset.read_from_hdx(dataset_filter)
+    resources = dataset.get_resources()
+    download_paths = []
+    for resource in resources:
+        if fnmatch.fnmatch(resource["name"], resource_filter):
+            expected_file_path = os.path.join(download_directory, f"{resource['name']}")
+            if os.path.exists(expected_file_path):
+                print(f"Expected file {expected_file_path} is already present, continuing")
+                download_paths.append(expected_file_path)
+            else:
+                print(f"Downloading {resource['name']}...")
+                resource_url, resource_file = resource.download(folder=download_directory)
+                print(f"...from {resource_url}")
+                download_paths.append(resource_file)
+
+    return download_paths
+
+
+def configure_hdx_connection(hdx_site: str, verbose: bool = True):
+    try:
+        Configuration.create(
+            user_agent_config_yaml=os.path.join(os.path.expanduser("~"), ".useragents.yaml"),
+            user_agent_lookup="hdx-cli-toolkit",
+            hdx_site=hdx_site,
+            hdx_read_only=False,
+        )
+        if verbose:
+            print(f"Connected to HDX site {Configuration.read().get_hdx_site_url()}", flush=True)
+    except ConfigurationError:
+        pass
```

### Comparing `hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit/hdx_utilities.py` & `hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,358 +1,531 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
-
-import fnmatch
-import json
-import os
-import time
-import traceback
-import yaml
-from hdx.api.configuration import Configuration, ConfigurationError
-from hdx.data.organization import Organization
-from hdx.data.resource_view import ResourceView
-from hdx.data.hdxobject import HDXError
-from hdx.data.dataset import Dataset
-from hdx.data.showcase import Showcase
-from hdx.data.resource import Resource
-from hdx.data.user import User
-
-from hdx_cli_toolkit.utilities import read_attributes
-
-
-def get_filtered_datasets(
-    organization: str = "",
-    dataset_filter: str = "*",
-    query: str = None,
-    hdx_site: str = "stage",
-    verbose: bool = True,
-) -> list[Dataset]:
-    """A function to return a list of datasets selected by some selection criteria based on
-    organization, dataset name, or CKAN query strings. The verbose flag is provided so
-    summary output can be suppressed for output to file in the print command.
-
-    Keyword Arguments:
-        organization {str} -- an organization name (default: {""})
-        key {str} -- _description_ (default: {"private"})
-        value {str} -- _description_ (default: {"value"})
-        dataset_filter {str} -- a filter for dataset name, can contain wildcards (default: {"*"})
-        query {str} -- a query string to use in the CKAN search API (default: {None})
-        hdx_site {str} -- target HDX site {prod|stage} (default: {"stage"})
-        verbose {bool} -- if True prints summary information (default: {True})
-
-    Returns:
-        list[Dataset] -- a list of datasets satisfying the selection criteria
-    """
-    configure_hdx_connection(hdx_site=hdx_site, verbose=False)
-
-    if organization != "":
-        organization = Organization.read_from_hdx(organization)
-        datasets = organization.get_datasets(include_private=True)
-    elif query is not None:
-        datasets = Dataset.search_in_hdx(query=query)
-        organization = {"display_name": "", "name": ""}
-    else:
-        dataset = Dataset.read_from_hdx(dataset_filter)
-        if dataset is None:
-            datasets = []
-            organization = {"display_name": "", "name": ""}
-        else:
-            datasets = [dataset]
-            organization = dataset.get_organization()
-            organization = {"display_name": organization["title"], "name": organization["name"]}
-
-    filtered_datasets = []
-    for dataset in datasets:
-        if fnmatch.fnmatch(dataset["name"], dataset_filter):
-            filtered_datasets.append(dataset)
-
-    if verbose:
-        print(Configuration.read().hdx_site, flush=True)
-        print(
-            f"Found {len(filtered_datasets)} datasets for organization "
-            f"'{organization['display_name']} "
-            f"({organization['name']})' matching filter conditions:",
-            flush=True,
-        )
-
-    return filtered_datasets
-
-
-def update_values_in_hdx(
-    filtered_datasets: list[Dataset], key, value, conversion_func, hdx_site: str = "stage"
-):
-    n_changed = 0
-    n_failures = 0
-    for dataset in filtered_datasets:
-        t0 = time.time()
-        old_value = str(dataset[key])
-        dataset[key] = conversion_func(value)
-        if old_value != str(dataset[key]):
-            n_changed += 1
-        else:
-            print(
-                f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20}"
-                f"{'No update required':<25.25}",
-                flush=True,
-            )
-            continue
-        try:
-            dataset.update_in_hdx(
-                update_resources=False,
-                hxl_update=False,
-                operation="patch",
-                batch_mode="KEEP_OLD",
-                skip_validation=True,
-                ignore_check=True,
-            )
-            print(
-                f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20}"
-                f"{time.time()-t0:0.2f}",
-                flush=True,
-            )
-        except (HDXError, KeyError):
-            if "Authorization Error" in traceback.format_exc():
-                print(
-                    f"Could not update {dataset['name']} on '{hdx_site}' "
-                    "because of an Authorization Error",
-                    flush=True,
-                )
-            else:
-                print(f"Could not update {dataset['name']} on '{hdx_site}'", flush=True)
-            n_failures += 1
-
-            print(
-                f"{dataset['name']:<70.70}{old_value:<20.20}{old_value:<20.20}"
-                f"{time.time()-t0:0.2f}",
-                flush=True,
-            )
-
-    return n_changed, n_failures
-
-
-def get_organizations_from_hdx(organization: str, hdx_site: str = "stage"):
-    configure_hdx_connection(hdx_site)
-    filtered_organizations = []
-    all_organizations = Organization.get_all_organization_names(include_extras=True)
-    for an_organization in all_organizations:
-        if fnmatch.fnmatch(an_organization, f"*{organization}*"):
-            organization_metadata = Organization.read_from_hdx(an_organization)
-            filtered_organizations.append(organization_metadata)
-
-    return filtered_organizations
-
-
-def get_users_from_hdx(user: str, hdx_site: str = "stage"):
-    configure_hdx_connection(hdx_site=hdx_site)
-
-    user_list = User.get_all_users(q=user)
-
-    return user_list
-
-
-def decorate_dataset_with_extras(
-    dataset: Dataset, hdx_site: str = "stage", verbose: bool = False
-) -> dict:
-    """A function to add resource, quickcharts (resource_view) and showcases keys to a dataset
-    dictionary representation for the print command. fs_check_info and hxl_preview_config are
-    converted from JSON objects serialised as single strings to dictionaries to make printed output
-    more readable. This decoration means that the dataset dictionary cannot be uploaded to HDX.
-
-    Arguments:
-        dataset {Dataset} -- a Dataset object to process
-
-    Returns:
-        dict -- a dictionary containing the dataset metadata
-    """
-    configure_hdx_connection(hdx_site, verbose=verbose)
-    output_dict = dataset.data
-    resources = dataset.get_resources()
-    output_dict["resources"] = []
-    for resource in resources:
-        resource_dict = resource.data
-        if "fs_check_info" in resource_dict:
-            resource_dict["fs_check_info"] = json.loads(resource_dict["fs_check_info"])
-        dataset_quickcharts = ResourceView.get_all_for_resource(resource_dict["id"])
-        resource_dict["quickcharts"] = []
-        if dataset_quickcharts is not None:
-            for quickchart in dataset_quickcharts:
-                quickchart_dict = quickchart.data
-                if "hxl_preview_config" in quickchart_dict:
-                    quickchart_dict["hxl_preview_config"] = json.loads(
-                        quickchart_dict["hxl_preview_config"]
-                    )
-                resource_dict["quickcharts"].append(quickchart_dict)
-        output_dict["resources"].append(resource_dict)
-
-    showcases = dataset.get_showcases()
-    output_dict["showcases"] = [x.data for x in showcases]
-
-    return output_dict
-
-
-def add_showcase(showcase_name: str, hdx_site: str, attributes_file_path: str) -> list[str]:
-    configure_hdx_connection(hdx_site)
-    statuses = []
-    showcase_attributes = read_attributes(showcase_name, attributes_filepath=attributes_file_path)
-    showcase = Showcase(
-        {
-            "name": showcase_attributes["name"],
-            "title": showcase_attributes["title"],
-            "notes": showcase_attributes["notes"],
-            "url": showcase_attributes["url"],
-            "image_url": showcase_attributes["image_url"],
-        }
-    )
-    added_tags, unadded_tags = showcase.add_tags(showcase_attributes["tags"])
-    statuses.append(f"{len(added_tags)} of {len(showcase_attributes['tags'])} showcase tags added")
-    if len(unadded_tags) != 0:
-        statuses.append(f"Rejected showcase tags: {unadded_tags}")
-
-    showcase.create_in_hdx()
-    dataset = Dataset.read_from_hdx(showcase_attributes["parent_dataset"])
-    showcase.add_dataset(dataset)
-    statuses.append(f"Added dataset '{dataset['name']}' to showcase '{showcase_name}'")
-
-    return statuses
-
-
-def update_resource_in_hdx(
-    dataset_name: str,
-    resource_name: str,
-    hdx_site: str,
-    resource_file_path: str,
-    live: bool,
-    description: str = "new resource",
-):
-    configure_hdx_connection(hdx_site)
-    statuses = []
-    dataset = Dataset.read_from_hdx(dataset_name)
-    # Check we found a dataset
-    if dataset is None:
-        statuses.append(f"No dataset with the name '{dataset_name}' found on HDX site '{hdx_site}'")
-        return statuses
-
-    statuses.append(f"Found dataset with the name '{dataset_name}' on HDX site '{hdx_site}'")
-    # Check we found a resource
-    resources = dataset.get_resources()
-    resource_to_update = None
-    for resource in resources:
-        if resource["name"] == resource_name:
-            resource_to_update = resource
-
-    # Report on the characteristics of the selected file for upload cf the original if available
-    if not os.path.exists(resource_file_path):
-        statuses.append(f"No file found at file path '{resource_file_path}'")
-        return statuses
-
-    statuses.append(f"Found file to upload at '{resource_file_path}'")
-
-    if resource_to_update is not None:
-        url = resource_to_update["url"]
-        original_filename = url[(url.rfind("/") + 1) :]  # noqa: E203
-        original_size = resource_to_update["size"]
-        statuses.append(
-            f"Original resource filename '{original_filename}' with size {original_size}"
-        )
-
-    replacement_filename = os.path.basename(resource_file_path)
-    file_stats = os.stat(resource_file_path)
-    replacement_size = file_stats.st_size
-    statuses.append(
-        f"Replacement resource filename '{replacement_filename}' with size {replacement_size}"
-    )
-
-    # This is the "add resource branch"
-    if resource_to_update is None:
-        statuses.append(
-            f"No resource with the name '{resource_name}' found on dataset '{dataset_name}', "
-            "adding file as new resource."
-        )
-        # Make a new resource
-        new_resource = Resource(
-            {
-                "name": resource_name,
-                "description": description,
-            }
-        )
-
-        new_resource.set_file_to_upload(resource_file_path, guess_format_from_suffix=True)
-        resource_list = [new_resource]
-        resource_list.extend(resources)
-        dataset.add_update_resources(resource_list, ignore_datasetid=True)
-        if live:
-            # It seems this match_resource_order keyword is not respected
-            dataset.update_in_hdx(match_resource_order=True)
-            # So we reload the dataset from HDX and force a reorder
-            revised_dataset = Dataset.read_from_hdx(dataset_name)
-            resources_check = revised_dataset.get_resources()
-
-            reordered_resource_ids = [
-                x["id"] for x in resources_check if x["name"] == resource_name
-            ]
-            reordered_resource_ids.extend(
-                [x["id"] for x in resources_check if x["name"] != resource_name]
-            )
-
-            revised_dataset.reorder_resources(resource_ids=reordered_resource_ids)
-            statuses.append("Addition to HDX successful")
-            return statuses
-    else:
-        resource_to_update.set_file_to_upload(resource_file_path, guess_format_from_suffix=True)
-        if live:
-            resource_to_update.update_in_hdx()
-            statuses.append("Update to HDX successful")
-            return statuses
-
-    statuses.append("No '--live' flag supplied so no update to HDX made, otherwise successful")
-    return statuses
-
-
-def add_quickcharts(dataset_name, hdx_site, resource_name, hdx_hxl_preview_file_path):
-    configure_hdx_connection(hdx_site=hdx_site)
-    status = "Successful"
-
-    # read the json file
-    with open(hdx_hxl_preview_file_path, "r", encoding="utf-8") as json_file:
-        recipe = json.load(json_file)
-    # extract appropriate keys
-    processed_recipe = {
-        "description": "",
-        "title": "Quick Charts",
-        "view_type": "hdx_hxl_preview",
-        "hxl_preview_config": "",
-    }
-
-    # convert the configuration to a string
-    stringified_config = json.dumps(
-        recipe["hxl_preview_config"], indent=None, separators=(",", ":")
-    )
-    processed_recipe["hxl_preview_config"] = stringified_config
-    # write out yaml to a temp file
-    temp_yaml_path = f"{hdx_hxl_preview_file_path}.temp.yaml"
-    with open(temp_yaml_path, "w", encoding="utf-8") as yaml_file:
-        yaml.dump(processed_recipe, yaml_file)
-
-    dataset = Dataset.read_from_hdx(dataset_name)
-    dataset.generate_quickcharts(resource=resource_name, path=temp_yaml_path)
-    dataset.update_in_hdx(update_resources=False, hxl_update=False)
-
-    # delete the temp file
-    if os.path.exists(temp_yaml_path):
-        os.remove(temp_yaml_path)
-
-    return status
-
-
-def configure_hdx_connection(hdx_site: str, verbose: bool = True):
-    try:
-        Configuration.create(
-            user_agent_config_yaml=os.path.join(os.path.expanduser("~"), ".useragents.yaml"),
-            user_agent_lookup="hdx-cli-toolkit",
-            hdx_site=hdx_site,
-            hdx_read_only=False,
-        )
-        if verbose:
-            print(f"Connected to HDX site {Configuration.read().get_hdx_site_url()}", flush=True)
-    except ConfigurationError:
-        pass
+#!/usr/bin/env python
+# encoding: utf-8
+
+import json
+import os
+import time
+
+from collections.abc import Callable
+
+import click
+from click.decorators import FC
+
+from hdx.api.configuration import ConfigurationError
+from hdx.utilities.path import script_dir_plus_file
+
+from hdx_cli_toolkit.utilities import (
+    write_dictionary,
+    print_table_from_list_of_dicts,
+    censor_secret,
+    make_conversion_func,
+    print_banner,
+)
+
+from hdx_cli_toolkit.hdx_utilities import (
+    add_showcase,
+    add_quickcharts,
+    get_organizations_from_hdx,
+    get_users_from_hdx,
+    update_values_in_hdx,
+    configure_hdx_connection,
+    update_resource_in_hdx,
+    get_filtered_datasets,
+    decorate_dataset_with_extras,
+    download_hdx_datasets,
+)
+
+
+@click.group()
+def hdx_toolkit() -> None:
+    """Tools for Commandline interactions with HDX"""
+
+
+OPTIONS = [
+    click.option(
+        "--organization",
+        is_flag=False,
+        default="",
+        help="an organization name",
+    ),
+    click.option(
+        "--key",
+        is_flag=False,
+        default="private",
+        help="a single key to list alongside organization",
+    ),
+    click.option(
+        "--value",
+        is_flag=False,
+        default=None,
+        help="a value to set",
+    ),
+    click.option(
+        "--dataset_filter",
+        is_flag=False,
+        default="*",
+        help="a dataset name or pattern on which to filter list",
+    ),
+    click.option(
+        "--query",
+        is_flag=False,
+        default=None,
+        help=(
+            "a dataset query string to pass to CKAN, "
+            "organization and dataset_filter are ignored if it is provided"
+        ),
+    ),
+    click.option(
+        "--hdx_site",
+        is_flag=False,
+        default="stage",
+        help="an hdx_site value {stage|prod}",
+    ),
+]
+
+
+def multi_decorator(options: list[Callable[[FC], FC]]) -> Callable[[FC], FC]:
+    def decorator(f: FC) -> FC:
+        for option in reversed(options):
+            f = option(f)
+
+        return f
+
+    return decorator
+
+
+@hdx_toolkit.command(name="list")
+@multi_decorator(OPTIONS)
+@click.option(
+    "--output_path",
+    is_flag=False,
+    default=None,
+    help="A file path to export data from list to CSV",
+)
+def list_datasets(
+    organization: str = "",
+    key: str = "private",
+    value: str = "value",
+    dataset_filter: str = "*",
+    query: str = None,
+    hdx_site: str = "stage",
+    output_path: str = None,
+):
+    """List datasets in HDX"""
+    print_banner("list")
+
+    filtered_datasets = get_filtered_datasets(
+        organization=organization,
+        dataset_filter=dataset_filter,
+        query=query,
+        hdx_site=hdx_site,
+    )
+
+    keys = key.split(",")
+    output_template = {"dataset_name": ""}
+    for key_ in keys:
+        output_template[key_] = ""
+
+    output = []
+    for dataset in filtered_datasets:
+        output_row = output_template.copy()
+        output_row["dataset_name"] = dataset["name"]
+        for key_ in keys:
+            output_row[key_] = dataset.get(key_, "")
+        output.append(output_row)
+
+    print_table_from_list_of_dicts(output)
+    if output_path is not None:
+        status = write_dictionary(output_path, output, append=False)
+        print(status, flush=True)
+
+
+@hdx_toolkit.command(name="update")
+@multi_decorator(OPTIONS)
+def update(
+    organization: str = "",
+    key: str = "private",
+    value: str = "value",
+    dataset_filter: str = "*",
+    query: str = None,
+    hdx_site: str = "stage",
+):
+    """Update datasets in HDX"""
+    print_banner("Update")
+    filtered_datasets = get_filtered_datasets(
+        organization=organization,
+        dataset_filter=dataset_filter,
+        query=query,
+        hdx_site=hdx_site,
+    )
+
+    if len(filtered_datasets) == 0:
+        print("Specified filter returns no datasets", flush=True)
+        return
+
+    print(f"Updating key '{key}' with value '{value}'")
+    conversion_func, type_name = make_conversion_func(filtered_datasets[0][key])
+    if conversion_func is None:
+        print(f"Type name '{type_name}' is not recognised, aborting", flush=True)
+        return
+
+    print(f"Detected value type is '{type_name}'", flush=True)
+    print(
+        f"{'dataset_name':<70.70}{'old value':<20.20}{'new value':<20.20}"
+        f"{'Time to update/seconds':<25.25}",
+        flush=True,
+    )
+    n_changed, n_failures = update_values_in_hdx(
+        filtered_datasets, key, value, conversion_func, hdx_site=hdx_site
+    )
+
+    print(f"Changed {n_changed} values", flush=True)
+    print(f"{n_failures} failures as evidenced by HDXError", flush=True)
+
+
+@hdx_toolkit.command(name="print")
+@multi_decorator(OPTIONS)
+@click.option(
+    "--with_extras",
+    is_flag=True,
+    default=False,
+    help=(
+        "If set resources, resource_views (QuickCharts) "
+        "and Showcases are added to the dataset output"
+    ),
+)
+def print_datasets(
+    organization: str = "healthsites",
+    key: str = "private",
+    value: str = "value",
+    dataset_filter: str = "*",
+    query: str = None,
+    hdx_site: str = "stage",
+    with_extras: bool = False,
+):
+    """Print datasets in HDX to the terminal"""
+
+    filtered_datasets = get_filtered_datasets(
+        organization=organization,
+        dataset_filter=dataset_filter,
+        hdx_site=hdx_site,
+        query=query,
+        verbose=False,
+    )
+
+    print("[", flush=True)
+    for i, dataset in enumerate(filtered_datasets):
+        output_dict = dataset.data
+        if with_extras:
+            output_dict = decorate_dataset_with_extras(dataset)
+
+        print(json.dumps(output_dict, indent=4), flush=True)
+        if i != len(filtered_datasets) - 1:
+            print(",", flush=True)
+    print("]", flush=True)
+
+
+@hdx_toolkit.command(name="get_organization_metadata")
+@click.option(
+    "--organization",
+    is_flag=False,
+    default="",
+    help="an organization name, wildcards are implicitly included",
+)
+@click.option(
+    "--hdx_site",
+    is_flag=False,
+    default="stage",
+    help="an hdx_site value {stage|prod}",
+)
+@click.option(
+    "--verbose",
+    is_flag=True,
+    default=False,
+    help="if true show all organization metadata",
+)
+def get_organization_metadata(organization: str, hdx_site: str = "stage", verbose: bool = False):
+    """Get an organization id and other metadata"""
+    print_banner("Get organization Metadata")
+    configure_hdx_connection(hdx_site=hdx_site)
+
+    filtered_organizations = get_organizations_from_hdx(organization, hdx_site=hdx_site)
+    for filtered_organization in filtered_organizations:
+        if verbose:
+            print(json.dumps(filtered_organization.data, indent=2), flush=True)
+        else:
+            print(
+                f"{filtered_organization['name']:<50.50}: {filtered_organization['id']}",
+                flush=True,
+            )
+
+
+@hdx_toolkit.command(name="get_user_metadata")
+@click.option(
+    "--user",
+    is_flag=False,
+    default="",
+    help="a user name or email, wildcards are implicitly included",
+)
+@click.option(
+    "--hdx_site",
+    is_flag=False,
+    default="stage",
+    help="an hdx_site value {stage|prod}",
+)
+@click.option(
+    "--verbose",
+    is_flag=True,
+    default=False,
+    help="if true show all user metadata",
+)
+def get_user_metadata(user: str, hdx_site: str = "stage", verbose: bool = False):
+    """Get user id and other metadata"""
+    print_banner("Get User Metadata")
+
+    user_list = get_users_from_hdx(user, hdx_site=hdx_site)
+    for a_user in user_list:
+        if verbose:
+            print(json.dumps(a_user.data, indent=2), flush=True)
+        else:
+            print(
+                f"{a_user['name']:<50.50}: {a_user['id']}",
+                flush=True,
+            )
+
+
+@hdx_toolkit.command(name="configuration")
+def show_configuration():
+    """Print configuration information to terminal"""
+    print_banner("configuration")
+    # Check files
+    user_hdx_config_yaml = os.path.join(os.path.expanduser("~"), ".hdx_configuration.yaml")
+    default_hdx_config_yaml = script_dir_plus_file(
+        "hdx_base_configuration.yaml", ConfigurationError
+    )
+
+    if os.path.exists(user_hdx_config_yaml):
+        click.secho(
+            f"Found a user configuration file at {user_hdx_config_yaml}. "
+            "Contents (secrets censored):",
+            bold=True,
+        )
+        with open(user_hdx_config_yaml, encoding="utf-8") as config_file:
+            config_file_contents = config_file.read()
+            rows = config_file_contents.split("\n")
+            for row in rows:
+                if row.startswith("hdx_key"):
+                    key_part, secret_part = row.split(":")
+                    secret_part = censor_secret(secret_part)
+                    row = key_part + ': "' + secret_part
+                print(row, flush=True)
+
+    user_agent_config_yaml = os.path.join(os.path.expanduser("~"), ".useragents.yaml")
+    if os.path.exists(user_agent_config_yaml):
+        click.secho(f"User agents file found at {user_agent_config_yaml}", bold=True)
+        with open(user_agent_config_yaml, encoding="utf-8") as config_file:
+            user_agents_file_contents = config_file.read()
+            print(user_agents_file_contents, flush=True)
+
+    # Check Environment variables
+    environment_variables = ["HDX_KEY", "HDX_KEY_STAGE", "HDX_SITE", "HDX_URL"]
+    click.secho(
+        "Values of relevant environment variables (used in absence of supplied values):", bold=True
+    )
+    for variable in environment_variables:
+        env_variable = os.getenv(variable)
+        if env_variable is not None:
+            if "HDX_KEY" in variable:
+                env_variable = censor_secret(env_variable)
+            print(f"{variable}:{env_variable}", flush=True)
+        else:
+            print(f"{variable} is not set", flush=True)
+
+    click.secho(
+        f"\nDefault base configuration file is at {default_hdx_config_yaml}. Contents:", bold=True
+    )
+    with open(default_hdx_config_yaml, encoding="utf-8") as config_file:
+        config_file_contents = config_file.read()
+        print(config_file_contents, flush=True)
+
+
+@hdx_toolkit.command(name="quickcharts")
+@click.option(
+    "--dataset_filter",
+    is_flag=False,
+    default="*",
+    help="a dataset name",
+)
+@click.option(
+    "--hdx_site",
+    is_flag=False,
+    default="stage",
+    help="an hdx_site value {stage|prod}",
+)
+@click.option(
+    "--resource_name",
+    is_flag=False,
+    default="stage",
+    help="name of resource to which the QuickCharts are attached",
+)
+@click.option(
+    "--hdx_hxl_preview_file_path",
+    is_flag=False,
+    default="stage",
+    help="name of resource to which the QuickCharts are attached",
+)
+def quickcharts(
+    dataset_filter: str = "",
+    hdx_site: str = "stage",
+    resource_name: str = "",
+    hdx_hxl_preview_file_path: str = "",
+):
+    """Upload QuickChart JSON description to HDX"""
+    print_banner("quickcharts")
+    print(
+        f"Adding Quick Chart defined at '{hdx_hxl_preview_file_path}' to dataset "
+        f"'{dataset_filter}', resource '{resource_name}'"
+    )
+    t0 = time.time()
+    status = add_quickcharts(dataset_filter, hdx_site, resource_name, hdx_hxl_preview_file_path)
+
+    print(status, flush=True)
+
+    print(f"Quick Chart update took {time.time() - t0:.2f} seconds")
+
+
+@hdx_toolkit.command(name="showcase")
+@click.option(
+    "--showcase_name",
+    is_flag=False,
+    default="*",
+    help="showcase name",
+)
+@click.option(
+    "--hdx_site",
+    is_flag=False,
+    default="stage",
+    help="an hdx_site value {stage|prod}",
+)
+@click.option(
+    "--attributes_file_path",
+    is_flag=False,
+    default="stage",
+    help="path to the attributes file describing the showcase",
+)
+def showcase(
+    showcase_name: str = "",
+    hdx_site: str = "stage",
+    attributes_file_path: str = "",
+):
+    """Upload showcase to HDX"""
+    print_banner("showcase")
+    print(f"Adding showcase defined at '{attributes_file_path}'")
+    t0 = time.time()
+    statuses = add_showcase(showcase_name, hdx_site, attributes_file_path)
+    for status in statuses:
+        print(status, flush=True)
+
+    print(f"Showcase update took {time.time() - t0:.2f} seconds")
+
+
+@hdx_toolkit.command(name="update_resource")
+@click.option(
+    "--dataset_name",
+    is_flag=False,
+    default="*",
+    help="name of the dataset to update",
+)
+@click.option(
+    "--resource_name",
+    is_flag=False,
+    default="*",
+    help="name of the resource in the dataset to update",
+)
+@click.option(
+    "--hdx_site",
+    is_flag=False,
+    default="stage",
+    help="an hdx_site value {stage|prod}",
+)
+@click.option(
+    "--resource_file_path",
+    is_flag=False,
+    default="stage",
+    help="path to the resource file to upload",
+)
+@click.option(
+    "--live",
+    is_flag=True,
+    default=False,
+    help="if present then update to HDX is made, if absent then a dry run is done",
+)
+@click.option(
+    "--description",
+    is_flag=False,
+    default="new resource",
+    help="if the resource is to be added, rather than updated this provides the description",
+)
+def update_resource(
+    dataset_name: str = "",
+    resource_name: str = "",
+    hdx_site: str = "stage",
+    resource_file_path: str = "",
+    live: bool = False,
+    description: str = "new resource",
+):
+    """Update a resource in HDX"""
+    print_banner("Update resource")
+    print(
+        f"Updating/adding '{resource_name}' in '{dataset_name}' "
+        f"with file at '{resource_file_path}'"
+    )
+    t0 = time.time()
+    statuses = update_resource_in_hdx(
+        dataset_name, resource_name, hdx_site, resource_file_path, live, description=description
+    )
+    for status in statuses:
+        print(status, flush=True)
+
+    print(f"Resource update took {time.time() - t0:.2f} seconds")
+
+
+@hdx_toolkit.command(name="download")
+@click.option(
+    "--dataset",
+    is_flag=False,
+    default="all",
+    help="target dataset for download",
+)
+@click.option(
+    "--resource_filter",
+    is_flag=False,
+    default="*",
+    help=("a resource name filter"),
+)
+@click.option(
+    "--hdx_site",
+    type=click.Choice(["stage", "prod"]),
+    is_flag=False,
+    default="stage",
+    help="an hdx_site value",
+)
+@click.option("--download_directory", is_flag=False, default=None, help="target_directory")
+def download(
+    dataset: str = "",
+    resource_filter: str = "*",
+    hdx_site: str = "stage",
+    download_directory: str = None,
+):
+    """Download dataset resources from HDX"""
+    print_banner("download")
+    if download_directory is None:
+        download_directory = os.path.join(os.path.dirname(__file__), "output")
+    download_paths = download_hdx_datasets(
+        dataset_filter=dataset,
+        resource_filter=resource_filter,
+        hdx_site=hdx_site,
+        download_directory=download_directory,
+    )
+    print("The following files were downloaded:", flush=True)
+    for download_path in download_paths:
+        print(download_path, flush=True)
```

### Comparing `hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit/utilities.py` & `hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/utilities.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,284 +1,284 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
-import csv
-import dataclasses
-import datetime
-import json
-import os
-
-from collections.abc import Callable
-from typing import Any
-
-import click
-
-
-def write_dictionary(
-    output_filepath: str, output_rows: list[dict[str, Any]], append: bool = True
-) -> str:
-    """Write a list of dictionaries to a CSV file
-
-    Arguments:
-        output_filepath {str} -- a file path for the output CSV file
-        output_rows {list[dict[str, Any]]} -- a list of dictionaries
-
-    Keyword Arguments:
-        append {bool} -- if True rows are appended to an existing file (default: {True})
-
-    Returns:
-        str -- a status message
-    """
-    keys = list(output_rows[0].keys())
-    newfile = not os.path.isfile(output_filepath)
-
-    if not append and not newfile:
-        os.remove(output_filepath)
-        newfile = True
-
-    with open(output_filepath, "a", encoding="utf-8", errors="ignore") as output_file:
-        dict_writer = csv.DictWriter(
-            output_file,
-            keys,
-            lineterminator="\n",
-        )
-        if newfile:
-            dict_writer.writeheader()
-        dict_writer.writerows(output_rows)
-
-    status = _make_write_dictionary_status(append, output_filepath, newfile)
-
-    return status
-
-
-def _make_write_dictionary_status(append: bool, filepath: str, newfile: bool) -> str:
-    """A simple helper function to generate a status message for write_dictionary
-
-    Arguments:
-        append {bool} -- the append flag
-        filepath {str} -- the file path for the output CSV file
-        newfile {bool} -- a file indicating whether a newfile was created
-
-    Returns:
-        str -- a status string
-    """
-    status = ""
-    if not append and not newfile:
-        status = f"Append is False, and {filepath} exists therefore file is being deleted"
-    elif not newfile and append:
-        status = f"Append is True, and {filepath} exists therefore data is being appended"
-    else:
-        status = f"New file {filepath} is being created"
-    return status
-
-
-def print_table_from_list_of_dicts(
-    column_data_rows: list[dict],
-    excluded_fields: None | list = None,
-    included_fields: None | list = None,
-    truncate_width: int = 130,
-    max_total_width: int = 150,
-) -> None:
-    """A helper function to print a list of dictionaries as a table
-
-    Arguments:
-        column_data_rows {list[dict]} -- the list of dictionaries to print
-
-    Keyword Arguments:
-        excluded_fields {None|list} -- any fields to be ommitted, none excluded by default
-                                        (default: {None})
-        included_fields {None|list} -- any fields to be included, all included by default
-                                        (default: {None})
-        truncate_width {int} -- width at which to truncate a column (default: {130})
-        max_total_width {int} -- total width of the table (default: {150})
-    """
-    if (len(column_data_rows)) == 0:
-        return
-    if dataclasses.is_dataclass(column_data_rows[0]):
-        temp_data = []
-        for row in column_data_rows:
-            temp_data.append(dataclasses.asdict(row))
-        column_data_rows = temp_data
-
-    if excluded_fields is None:
-        excluded_fields = []
-
-    if included_fields is None:
-        included_fields = list(column_data_rows[0])
-
-    column_table_header_dict = {}
-    for field in included_fields:
-        widths = [len(str(x[field])) for x in column_data_rows]
-        widths.append(len(field))  # .append(len(field))
-        max_field_width = max(widths)
-
-        column_table_header_dict[field] = max_field_width + 1
-        if max_field_width > truncate_width:
-            column_table_header_dict[field] = truncate_width
-
-    total_width = (
-        sum(v for k, v in column_table_header_dict.items() if k not in excluded_fields)
-        + len(column_table_header_dict)
-        - 1
-    )
-
-    if total_width > max_total_width:
-        print(
-            f"\nCalculated total_width of {total_width} "
-            f"exceeds proposed max_total_width of {max_total_width}. "
-            "The resulting table may be unattractive.",
-            flush=True,
-        )
-
-    print("-" * total_width, flush=True)
-
-    for k in included_fields:
-        if k not in excluded_fields:
-            width = column_table_header_dict[k]
-            print(f"|{k:<{width}.{width}}", end="", flush=True)
-    print("|", flush=True)
-    print("-" * total_width, flush=True)
-
-    for row in column_data_rows:
-        for k in included_fields:
-            value = row[k]
-
-            if k not in excluded_fields:
-                width = column_table_header_dict[k]
-                print(f"|{str(value):<{width}.{width}}", end="", flush=True)
-        print("|", flush=True)
-
-    print("-" * total_width, flush=True)
-
-
-def censor_secret(secret: str) -> str:
-    """A function to censor a string containing a secret. If the length of the string is less than
-    10 characters then all characters are censored, if it is more then the last 10 characters are
-    left in place.
-
-    Arguments:
-        secret {str} -- a secret
-
-    Returns:
-        str -- the secret, censored
-    """
-    if len(secret) < 10:
-        censored_secret = len(secret) * "*"
-    else:
-        censored_secret = (len(secret) - 10) * "*" + secret[-10:]
-    return censored_secret
-
-
-def str_to_bool(x: str) -> bool:
-    """A function that converts a string into a boolean using the formalism that any casing of the
-    string "True" is True and all other strings are False. The default behaviour of the builtin
-    bool is that any non-empty string is True
-
-    Arguments:
-        x {str} -- a string
-
-    Returns:
-        bool -- a boolean representation of the string
-    """
-    return x.lower() == "true"
-
-
-def make_conversion_func(value: Any) -> tuple[Callable | None, str]:
-    """A function that takes a value of Any type and returns the function that will convert a string
-     to that type. Used to take values from dataset attributes and work out how to convert a string
-     from the commandline.
-
-    Arguments:
-        value {Any} -- a value of Any type
-
-    Returns:
-        tuple[Callable | None, str] -- a function that will convert a string to the provided type,
-                                       and the name of that type
-    """
-    value_type = type(value)
-    if value_type.__name__ == "bool":
-        conversion_func = str_to_bool
-    elif value_type.__name__ == "int":
-        conversion_func = int
-    elif value_type.__name__ == "float":
-        conversion_func = float
-    elif value_type.__name__ == "str":
-        conversion_func = str
-    else:
-        conversion_func = None
-
-    return conversion_func, value_type.__name__
-
-
-def read_attributes(dataset_name: str, attributes_filepath: str) -> dict:
-    """A function for reading attributes from a standard attributes.csv file with columns:
-    dataset_name,timestamp,attribute,value,secondary_value or a JSON format file containing
-    either a list or a single dictionary.
-
-    Arguments:
-        dataset_name {str} -- the name of the dataset for which attributes are required
-        attributes_filepath {str} -- path to attributes file either CSV or JSON
-
-    Returns:
-        dict -- a dictionary containing the attributes
-    """
-
-    if attributes_filepath.lower().endswith(".csv"):
-        with open(attributes_filepath, "r", encoding="UTF-8") as attributes_filehandle:
-            attribute_rows = csv.DictReader(attributes_filehandle)
-            attributes = {}
-
-            for row in attribute_rows:
-                if list(row.keys()) != [
-                    "dataset_name",
-                    "timestamp",
-                    "attribute",
-                    "value",
-                    "secondary_value",
-                ]:
-                    print(
-                        "Attributes.csv file must have columns: "
-                        "dataset_name, timestamp, attribute, value, secondary_value"
-                    )
-                    return attributes
-
-                if row["dataset_name"] != dataset_name:
-                    continue
-                if row["attribute"] in ["resource", "skip_country", "showcase", "tags"]:
-                    if row["attribute"] not in attributes:
-                        attributes[row["attribute"]] = [row["value"]]
-                    else:
-                        attributes[row["attribute"]].append(row["value"])
-                else:
-                    attributes[row["attribute"]] = row["value"]
-    elif attributes_filepath.lower().endswith(".json"):
-        with open(attributes_filepath, "r", encoding="utf-8") as attributes_filehandle:
-            raw_json = json.load(attributes_filehandle)
-            if isinstance(raw_json, dict):
-                attributes = raw_json
-            elif isinstance(raw_json, list):
-                for entry in raw_json:
-                    if entry["name"] == dataset_name:
-                        attributes = entry
-                        break
-
-    else:
-        print(f"File type at {attributes_filepath} is not recognised")
-        attributes = {}
-
-    return attributes
-
-
-def print_banner(action: str):
-    """Simple function to output a banner to console, uses click's secho command but not colour
-    because the underlying colorama does not output correctly to git-bash terminals.
-
-    Arguments:
-        action {str} -- _description_
-    """
-    title = f"HDX CLI toolkit - {action}"
-    timestamp = f"Invoked at: {datetime.datetime.now().isoformat()}"
-    width = max(len(title), len(timestamp))
-    click.secho((width + 4) * "*", bold=True)
-    click.secho(f"* {title:<{width}} *", bold=True)
-    click.secho(f"* {timestamp:<{width}} *", bold=True)
-    click.secho((width + 4) * "*", bold=True)
+#!/usr/bin/env python
+# encoding: utf-8
+
+import csv
+import dataclasses
+import datetime
+import json
+import os
+
+from collections.abc import Callable
+from typing import Any
+
+import click
+
+
+def write_dictionary(
+    output_filepath: str, output_rows: list[dict[str, Any]], append: bool = True
+) -> str:
+    """Write a list of dictionaries to a CSV file
+
+    Arguments:
+        output_filepath {str} -- a file path for the output CSV file
+        output_rows {list[dict[str, Any]]} -- a list of dictionaries
+
+    Keyword Arguments:
+        append {bool} -- if True rows are appended to an existing file (default: {True})
+
+    Returns:
+        str -- a status message
+    """
+    keys = list(output_rows[0].keys())
+    newfile = not os.path.isfile(output_filepath)
+
+    if not append and not newfile:
+        os.remove(output_filepath)
+        newfile = True
+
+    with open(output_filepath, "a", encoding="utf-8", errors="ignore") as output_file:
+        dict_writer = csv.DictWriter(
+            output_file,
+            keys,
+            lineterminator="\n",
+        )
+        if newfile:
+            dict_writer.writeheader()
+        dict_writer.writerows(output_rows)
+
+    status = _make_write_dictionary_status(append, output_filepath, newfile)
+
+    return status
+
+
+def _make_write_dictionary_status(append: bool, filepath: str, newfile: bool) -> str:
+    """A simple helper function to generate a status message for write_dictionary
+
+    Arguments:
+        append {bool} -- the append flag
+        filepath {str} -- the file path for the output CSV file
+        newfile {bool} -- a file indicating whether a newfile was created
+
+    Returns:
+        str -- a status string
+    """
+    status = ""
+    if not append and not newfile:
+        status = f"Append is False, and {filepath} exists therefore file is being deleted"
+    elif not newfile and append:
+        status = f"Append is True, and {filepath} exists therefore data is being appended"
+    else:
+        status = f"New file {filepath} is being created"
+    return status
+
+
+def print_table_from_list_of_dicts(
+    column_data_rows: list[dict],
+    excluded_fields: None | list = None,
+    included_fields: None | list = None,
+    truncate_width: int = 130,
+    max_total_width: int = 150,
+) -> None:
+    """A helper function to print a list of dictionaries as a table
+
+    Arguments:
+        column_data_rows {list[dict]} -- the list of dictionaries to print
+
+    Keyword Arguments:
+        excluded_fields {None|list} -- any fields to be ommitted, none excluded by default
+                                        (default: {None})
+        included_fields {None|list} -- any fields to be included, all included by default
+                                        (default: {None})
+        truncate_width {int} -- width at which to truncate a column (default: {130})
+        max_total_width {int} -- total width of the table (default: {150})
+    """
+    if (len(column_data_rows)) == 0:
+        return
+    if dataclasses.is_dataclass(column_data_rows[0]):
+        temp_data = []
+        for row in column_data_rows:
+            temp_data.append(dataclasses.asdict(row))
+        column_data_rows = temp_data
+
+    if excluded_fields is None:
+        excluded_fields = []
+
+    if included_fields is None:
+        included_fields = list(column_data_rows[0])
+
+    column_table_header_dict = {}
+    for field in included_fields:
+        widths = [len(str(x[field])) for x in column_data_rows]
+        widths.append(len(field))  # .append(len(field))
+        max_field_width = max(widths)
+
+        column_table_header_dict[field] = max_field_width + 1
+        if max_field_width > truncate_width:
+            column_table_header_dict[field] = truncate_width
+
+    total_width = (
+        sum(v for k, v in column_table_header_dict.items() if k not in excluded_fields)
+        + len(column_table_header_dict)
+        - 1
+    )
+
+    if total_width > max_total_width:
+        print(
+            f"\nCalculated total_width of {total_width} "
+            f"exceeds proposed max_total_width of {max_total_width}. "
+            "The resulting table may be unattractive.",
+            flush=True,
+        )
+
+    print("-" * total_width, flush=True)
+
+    for k in included_fields:
+        if k not in excluded_fields:
+            width = column_table_header_dict[k]
+            print(f"|{k:<{width}.{width}}", end="", flush=True)
+    print("|", flush=True)
+    print("-" * total_width, flush=True)
+
+    for row in column_data_rows:
+        for k in included_fields:
+            value = row[k]
+
+            if k not in excluded_fields:
+                width = column_table_header_dict[k]
+                print(f"|{str(value):<{width}.{width}}", end="", flush=True)
+        print("|", flush=True)
+
+    print("-" * total_width, flush=True)
+
+
+def censor_secret(secret: str) -> str:
+    """A function to censor a string containing a secret. If the length of the string is less than
+    10 characters then all characters are censored, if it is more then the last 10 characters are
+    left in place.
+
+    Arguments:
+        secret {str} -- a secret
+
+    Returns:
+        str -- the secret, censored
+    """
+    if len(secret) < 10:
+        censored_secret = len(secret) * "*"
+    else:
+        censored_secret = (len(secret) - 10) * "*" + secret[-10:]
+    return censored_secret
+
+
+def str_to_bool(x: str) -> bool:
+    """A function that converts a string into a boolean using the formalism that any casing of the
+    string "True" is True and all other strings are False. The default behaviour of the builtin
+    bool is that any non-empty string is True
+
+    Arguments:
+        x {str} -- a string
+
+    Returns:
+        bool -- a boolean representation of the string
+    """
+    return x.lower() == "true"
+
+
+def make_conversion_func(value: Any) -> tuple[Callable | None, str]:
+    """A function that takes a value of Any type and returns the function that will convert a string
+     to that type. Used to take values from dataset attributes and work out how to convert a string
+     from the commandline.
+
+    Arguments:
+        value {Any} -- a value of Any type
+
+    Returns:
+        tuple[Callable | None, str] -- a function that will convert a string to the provided type,
+                                       and the name of that type
+    """
+    value_type = type(value)
+    if value_type.__name__ == "bool":
+        conversion_func = str_to_bool
+    elif value_type.__name__ == "int":
+        conversion_func = int
+    elif value_type.__name__ == "float":
+        conversion_func = float
+    elif value_type.__name__ == "str":
+        conversion_func = str
+    else:
+        conversion_func = None
+
+    return conversion_func, value_type.__name__
+
+
+def read_attributes(dataset_name: str, attributes_filepath: str) -> dict:
+    """A function for reading attributes from a standard attributes.csv file with columns:
+    dataset_name,timestamp,attribute,value,secondary_value or a JSON format file containing
+    either a list or a single dictionary.
+
+    Arguments:
+        dataset_name {str} -- the name of the dataset for which attributes are required
+        attributes_filepath {str} -- path to attributes file either CSV or JSON
+
+    Returns:
+        dict -- a dictionary containing the attributes
+    """
+
+    if attributes_filepath.lower().endswith(".csv"):
+        with open(attributes_filepath, "r", encoding="UTF-8") as attributes_filehandle:
+            attribute_rows = csv.DictReader(attributes_filehandle)
+            attributes = {}
+
+            for row in attribute_rows:
+                if list(row.keys()) != [
+                    "dataset_name",
+                    "timestamp",
+                    "attribute",
+                    "value",
+                    "secondary_value",
+                ]:
+                    print(
+                        "Attributes.csv file must have columns: "
+                        "dataset_name, timestamp, attribute, value, secondary_value"
+                    )
+                    return attributes
+
+                if row["dataset_name"] != dataset_name:
+                    continue
+                if row["attribute"] in ["resource", "skip_country", "showcase", "tags"]:
+                    if row["attribute"] not in attributes:
+                        attributes[row["attribute"]] = [row["value"]]
+                    else:
+                        attributes[row["attribute"]].append(row["value"])
+                else:
+                    attributes[row["attribute"]] = row["value"]
+    elif attributes_filepath.lower().endswith(".json"):
+        with open(attributes_filepath, "r", encoding="utf-8") as attributes_filehandle:
+            raw_json = json.load(attributes_filehandle)
+            if isinstance(raw_json, dict):
+                attributes = raw_json
+            elif isinstance(raw_json, list):
+                for entry in raw_json:
+                    if entry["name"] == dataset_name:
+                        attributes = entry
+                        break
+
+    else:
+        print(f"File type at {attributes_filepath} is not recognised")
+        attributes = {}
+
+    return attributes
+
+
+def print_banner(action: str):
+    """Simple function to output a banner to console, uses click's secho command but not colour
+    because the underlying colorama does not output correctly to git-bash terminals.
+
+    Arguments:
+        action {str} -- _description_
+    """
+    title = f"HDX CLI toolkit - {action}"
+    timestamp = f"Invoked at: {datetime.datetime.now().isoformat()}"
+    width = max(len(title), len(timestamp))
+    click.secho((width + 4) * "*", bold=True)
+    click.secho(f"* {title:<{width}} *", bold=True)
+    click.secho(f"* {timestamp:<{width}} *", bold=True)
+    click.secho((width + 4) * "*", bold=True)
```

### Comparing `hdx_cli_toolkit-2024.3.4/src/hdx_cli_toolkit.egg-info/SOURCES.txt` & `hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 src/hdx_cli_toolkit/utilities.py
 src/hdx_cli_toolkit.egg-info/PKG-INFO
 src/hdx_cli_toolkit.egg-info/SOURCES.txt
 src/hdx_cli_toolkit.egg-info/dependency_links.txt
 src/hdx_cli_toolkit.egg-info/entry_points.txt
 src/hdx_cli_toolkit.egg-info/requires.txt
 src/hdx_cli_toolkit.egg-info/top_level.txt
-src/temp/resource_order_test.py
 tests/test_cli.py
+tests/test_cli_integration.py
 tests/test_hdx_utilities.py
-tests/test_integration.py
+tests/test_hdx_utilities_integration.py
 tests/test_utilities.py
```

### Comparing `hdx_cli_toolkit-2024.3.4/src/temp/resource_order_test.py` & `hdx_cli_toolkit-2024.4.1/tests/test_hdx_utilities_integration.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,116 @@
-#!/usr/bin/env python
-"""
-Creates a dataset on HDX.
-
-"""
-import logging
-from os.path import expanduser, join
-
-from hdx.data.dataset import Dataset
-from hdx.data.resource import Resource
-from hdx.facades.simple import facade
-from hdx.utilities.dateparse import parse_date
-
-logger = logging.getLogger(__name__)
-
-
-def main():
-
-    def create_dataset_metadata():
-        """Generate dataset and create it in HDX"""
-        dataset = Dataset(
-            {
-                "name": "reorder-test",
-                "title": "Reordering Test Dataset",
-                "license_id": "cc-by-igo",
-                "methodology": "Other",
-                "private": False,
-                "dataset_source": "Innago",
-            }
-        )
-        dataset["notes"] = "Long description of dataset goes here!"
-        dataset["methodology_other"] = "Describe methodology here!"
-        dataset["caveats"] = "Any caveats or comments about the data go here!"
-        dataset.set_maintainer("196196be-6037-4488-8b71-d786adf4c081")  # mcarans
-        dataset.set_organization("5a63012e-6c41-420c-8c33-e84b277fdc90")  # innago organisation
-        dataset.set_expected_update_frequency("Every year")
-        dataset.set_subnational(False)
-        dataset.add_tags(["geodata"])
-        dataset.set_time_period(parse_date("2020-03-05"), parse_date("2021-02-25"))
-
-        dataset.add_country_location("AFG")
-        return dataset
-
-    dataset = create_dataset_metadata()
-    # for i in range(10):
-    i = 0
-    name = f"resource-{i}"
-    resource = Resource({"name": name, "description": name, "format": "xlsx"})
-    resource.set_file_to_upload("test.xlsx")
-    dataset.add_update_resource(resource)
-
-    dataset.create_in_hdx()
-    logger.info("Dataset created!")
-
-    dataset = Dataset.read_from_hdx("reorder-test")
-    original_resources = dataset.get_resources()
-    for resource in original_resources:
-        logger.info(f"Resource name: {resource['name']}")
-
-    dataset = create_dataset_metadata()
-    name = "resource-inserted"
-    resource = Resource({"name": name, "description": name, "format": "xlsx"})
-    resource.set_file_to_upload("test-2.xlsx")
-
-    reordered_resources = [resource]
-    original_resources.reverse()
-    reordered_resources.extend(original_resources)
-    dataset.add_update_resources(reordered_resources, ignore_datasetid=True)
-    #
-
-    # for i in range(10):
-    #     name = f"resource-{9-i}"
-    #     resource = Resource({"name": name, "description": name, "format": "xlsx"})
-    #     resource.set_file_to_upload("test.xlsx")
-    #     dataset.add_update_resource(resource)
-
-    dataset.update_in_hdx(match_resource_order=True)
-    logger.info("Dataset updated!")
-
-    dataset = Dataset.read_from_hdx("reorder-test")
-    for resource in dataset.get_resources():
-        logger.info(f"Resource name: {resource['name']}")
-
-    dataset.delete_from_hdx()
-    logger.info("Dataset deleted!")
-
-
-if __name__ == "__main__":
-    facade(
-        main,
-        hdx_site="demo",
-        user_agent_config_yaml=join(expanduser("~"), ".useragents.yaml"),
-        user_agent_lookup="rename_datasets",
-    )
+#!/usr/bin/env python
+# encoding: utf-8
+
+# These tests interact directly with the staging HDX instance
+
+import json
+import os
+
+import pytest
+
+from hdx.data.dataset import Dataset
+from hdx.data.resource import Resource
+
+from hdx_cli_toolkit.hdx_utilities import update_resource_in_hdx, configure_hdx_connection
+
+
+DATASET_NAME = "hdx_cli_toolkit_test"
+TEST_RESOURCE_NAME = "test_resource_1"
+
+
+@pytest.fixture(autouse=True)
+def setup_and_teardown_dataset_in_hdx():
+    # This is pytest setup
+    configure_hdx_connection(hdx_site="stage")
+    dataset = Dataset.read_from_hdx(DATASET_NAME)
+    if dataset:
+        dataset.delete_from_hdx()
+    title = "HDX CLI toolkit test"
+    dataset = Dataset({"name": DATASET_NAME, "title": title})
+    dataset.update_from_yaml(
+        os.path.join(os.path.dirname(__file__), "fixtures", "hdx_dataset_static.yaml")
+    )
+    countryiso3s = ["AFG", "PSE", "SYR", "YEM"]
+    dataset.add_country_locations(countryiso3s)
+    tags = ["conflict-violence", "displacement", "hxl"]
+    dataset.add_tags(tags)
+
+    resource = Resource(
+        {
+            "name": TEST_RESOURCE_NAME,
+            "description": "Test Resource 1",
+        }
+    )
+    resource_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "test.csv")
+    resource.set_format("csv")
+    resource.set_file_to_upload(resource_file_path)
+
+    dataset.add_update_resource(resource)
+
+    dataset.create_in_hdx(hxl_update=False, updated_by_script="hdx_cli_toolkit_ignore")
+
+    assert Dataset.read_from_hdx(DATASET_NAME) is not None
+    # This is pytest teardown
+    yield
+    dataset = Dataset.read_from_hdx(DATASET_NAME)
+    if dataset:
+        dataset.delete_from_hdx()
+
+
+def test_update_resource():
+    dataset = Dataset.read_from_hdx(DATASET_NAME)
+    original_resources = dataset.get_resources()
+
+    new_resource_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "test-2.csv")
+    statuses = update_resource_in_hdx(
+        DATASET_NAME, TEST_RESOURCE_NAME, "stage", new_resource_file_path, live=True
+    )
+
+    for status in statuses:
+        print(status, flush=True)
+
+    assert len(statuses) == 5
+
+    revised_dataset = Dataset.read_from_hdx(DATASET_NAME)
+    revised_resources = revised_dataset.get_resources()
+
+    assert len(original_resources) == len(revised_resources)
+    assert original_resources[0].data["name"] == "test_resource_1"
+    assert revised_resources[0].data["name"] == "test_resource_1"
+
+    assert original_resources[0].data["url"].endswith("test.csv")
+    assert revised_resources[0].data["url"].endswith("test-2.csv")
+
+    assert revised_resources[0].data["size"] > original_resources[0].data["size"]
+
+
+def test_add_resource():
+    dataset = Dataset.read_from_hdx(DATASET_NAME)
+    original_resources = dataset.get_resources()
+    new_resource_name = "inserted_resource"
+
+    new_resource_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "test-2.csv")
+    statuses = update_resource_in_hdx(
+        DATASET_NAME, new_resource_name, "stage", new_resource_file_path, live=True
+    )
+
+    for status in statuses:
+        print(status, flush=True)
+
+    assert len(statuses) == 5
+
+    revised_dataset = Dataset.read_from_hdx(DATASET_NAME)
+    revised_resources = revised_dataset.get_resources()
+    for revised_ in revised_resources:
+        print(revised_["name"], flush=True)
+
+    assert len(original_resources) == 1
+    assert len(revised_resources) == 2
+
+    assert revised_resources[0].data["name"] == "inserted_resource"
+    assert revised_resources[1].data["name"] == "test_resource_1"
+
+    assert revised_resources[0].data["url"].endswith("test-2.csv")
+    assert revised_resources[1].data["url"].endswith("test.csv")
+
+    assert revised_resources[0].data["size"] > original_resources[0].data["size"]
```

### Comparing `hdx_cli_toolkit-2024.3.4/tests/test_utilities.py` & `hdx_cli_toolkit-2024.4.1/tests/test_utilities.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
-import csv
-import os
-
-from hdx_cli_toolkit.utilities import write_dictionary, censor_secret, read_attributes
-
-
-ATTRIBUTES_FILE_PATH = os.path.join(os.path.dirname(__file__), "fixtures", "attributes.csv")
-DATASET_NAME = "climada-litpop-showcase"
-REFERENCE_ATTRIBUTES = read_attributes(DATASET_NAME, attributes_filepath=ATTRIBUTES_FILE_PATH)
-
-
-def test_write_dictionary_to_local_file():
-    temp_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "test.csv")
-    if os.path.isfile(temp_file_path):
-        os.remove(temp_file_path)
-
-    dict_list = [
-        {"a": 1, "b": 2, "c": 3},
-        {"a": 4, "b": 5, "c": 6},
-        {"a": 7, "b": 8, "c": 9},
-    ]
-
-    status = write_dictionary(temp_file_path, dict_list)
-
-    with open(temp_file_path, "r", encoding="utf-8") as file_handle:
-        rows_read = list(csv.DictReader(file_handle))
-
-    assert len(rows_read) == 3
-    assert rows_read[0] == {"a": "1", "b": "2", "c": "3"}
-    assert "New file" in status
-    assert "is being created" in status
-
-
-def test_censor_short_secret():
-    censored_secret = censor_secret("012345")
-    assert censored_secret == "******"
-
-
-def test_censor_long_secret():
-    censored_secret = censor_secret("ABCDEF0123456789")
-    assert censored_secret == "******0123456789"
-
-
-def test_read_attributes():
-    assert len(REFERENCE_ATTRIBUTES["tags"]) == 3
-    assert REFERENCE_ATTRIBUTES["parent_dataset"] == "climada-litpop-dataset"
-
-
-def test_read_attributes_json():
-    attributes_json_file_path = os.path.join(
-        os.path.dirname(__file__), "fixtures", "attributes-single.json"
-    )
-
-    dataset_attributes = read_attributes(
-        DATASET_NAME, attributes_filepath=attributes_json_file_path
-    )
-
-    assert REFERENCE_ATTRIBUTES == dataset_attributes
-
-
-def test_read_attributes_json_list():
-    attributes_json_list_file_path = os.path.join(
-        os.path.dirname(__file__), "fixtures", "attributes-list.json"
-    )
-
-    dataset_attributes = read_attributes(
-        DATASET_NAME, attributes_filepath=attributes_json_list_file_path
-    )
-
-    assert REFERENCE_ATTRIBUTES == dataset_attributes
+#!/usr/bin/env python
+# encoding: utf-8
+
+import csv
+import os
+
+from hdx_cli_toolkit.utilities import write_dictionary, censor_secret, read_attributes
+
+
+ATTRIBUTES_FILE_PATH = os.path.join(os.path.dirname(__file__), "fixtures", "attributes.csv")
+DATASET_NAME = "climada-litpop-showcase"
+REFERENCE_ATTRIBUTES = read_attributes(DATASET_NAME, attributes_filepath=ATTRIBUTES_FILE_PATH)
+
+
+def test_write_dictionary_to_local_file():
+    temp_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "test.csv")
+    if os.path.isfile(temp_file_path):
+        os.remove(temp_file_path)
+
+    dict_list = [
+        {"a": 1, "b": 2, "c": 3},
+        {"a": 4, "b": 5, "c": 6},
+        {"a": 7, "b": 8, "c": 9},
+    ]
+
+    status = write_dictionary(temp_file_path, dict_list)
+
+    with open(temp_file_path, "r", encoding="utf-8") as file_handle:
+        rows_read = list(csv.DictReader(file_handle))
+
+    assert len(rows_read) == 3
+    assert rows_read[0] == {"a": "1", "b": "2", "c": "3"}
+    assert "New file" in status
+    assert "is being created" in status
+
+
+def test_censor_short_secret():
+    censored_secret = censor_secret("012345")
+    assert censored_secret == "******"
+
+
+def test_censor_long_secret():
+    censored_secret = censor_secret("ABCDEF0123456789")
+    assert censored_secret == "******0123456789"
+
+
+def test_read_attributes():
+    assert len(REFERENCE_ATTRIBUTES["tags"]) == 3
+    assert REFERENCE_ATTRIBUTES["parent_dataset"] == "climada-litpop-dataset"
+
+
+def test_read_attributes_json():
+    attributes_json_file_path = os.path.join(
+        os.path.dirname(__file__), "fixtures", "attributes-single.json"
+    )
+
+    dataset_attributes = read_attributes(
+        DATASET_NAME, attributes_filepath=attributes_json_file_path
+    )
+
+    assert REFERENCE_ATTRIBUTES == dataset_attributes
+
+
+def test_read_attributes_json_list():
+    attributes_json_list_file_path = os.path.join(
+        os.path.dirname(__file__), "fixtures", "attributes-list.json"
+    )
+
+    dataset_attributes = read_attributes(
+        DATASET_NAME, attributes_filepath=attributes_json_list_file_path
+    )
+
+    assert REFERENCE_ATTRIBUTES == dataset_attributes
```

