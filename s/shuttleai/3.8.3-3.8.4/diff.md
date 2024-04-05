# Comparing `tmp/shuttleai-3.8.3.tar.gz` & `tmp/shuttleai-3.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.8.3.tar", last modified: Fri Apr  5 20:15:23 2024, max compression
+gzip compressed data, was "shuttleai-3.8.4.tar", last modified: Fri Apr  5 20:22:18 2024, max compression
```

## Comparing `shuttleai-3.8.3.tar` & `shuttleai-3.8.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.827007 shuttleai-3.8.3/
--rw-rw-rw-   0        0        0     4184 2024-04-05 20:15:23.825009 shuttleai-3.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 20:15:23.827007 shuttleai-3.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1783 2024-04-05 17:17:27.000000 shuttleai-3.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.751008 shuttleai-3.8.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.761009 shuttleai-3.8.3/src/shuttleai/
--rw-rw-rw-   0        0        0      576 2024-04-05 20:15:18.000000 shuttleai-3.8.3/src/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.3/src/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.817010 shuttleai-3.8.3/src/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.3/src/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17420 2024-04-05 20:15:15.000000 shuttleai-3.8.3/src/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0    15283 2024-04-05 20:15:16.000000 shuttleai-3.8.3/src/shuttleai/client/_sync.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.3/src/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.820008 shuttleai-3.8.3/src/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.3/src/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     2030 2024-04-03 02:15:03.000000 shuttleai-3.8.3/src/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.823008 shuttleai-3.8.3/src/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     4184 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.384580 shuttleai-3.8.4/
+-rw-rw-rw-   0        0        0     4109 2024-04-05 20:22:18.382582 shuttleai-3.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 20:22:18.384580 shuttleai-3.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2024-04-05 20:21:42.000000 shuttleai-3.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.314577 shuttleai-3.8.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.322581 shuttleai-3.8.4/src/shuttleai/
+-rw-rw-rw-   0        0        0      576 2024-04-05 20:21:58.000000 shuttleai-3.8.4/src/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.4/src/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.373581 shuttleai-3.8.4/src/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.4/src/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17420 2024-04-05 20:22:01.000000 shuttleai-3.8.4/src/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0    15283 2024-04-05 20:22:03.000000 shuttleai-3.8.4/src/shuttleai/client/_sync.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.4/src/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.377581 shuttleai-3.8.4/src/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.4/src/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2030 2024-04-03 02:15:03.000000 shuttleai-3.8.4/src/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.379581 shuttleai-3.8.4/src/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     4109 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.8.3/PKG-INFO` & `shuttleai-3.8.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.3
+Version: 3.8.4
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: httpx
 Requires-Dist: aiohttp
+Requires-Dist: httpx
 Requires-Dist: orjson
 Requires-Dist: pydantic
 Provides-Extra: cli
-Requires-Dist: httpx; extra == "cli"
-Requires-Dist: aiohttp; extra == "cli"
-Requires-Dist: orjson; extra == "cli"
-Requires-Dist: pydantic; extra == "cli"
+Requires-Dist: asyncclick; extra == "cli"
+Requires-Dist: pystyle; extra == "cli"
 
 # The official Python library for the ShuttleAI API
 Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
 
 > *PRs appreciated 🙂*
 # Installation
 ## ShuttleAI
```

### Comparing `shuttleai-3.8.3/README.md` & `shuttleai-3.8.4/README.md`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.3/setup.py` & `shuttleai-3.8.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 from src.shuttleai import __version__ as version
 
-def read_requirements(file_path, extras=()):
-    requirements = []
-    with open(file_path, 'r') as file:
-        for line in file:
-            line = line.strip()
-            if line and not line.startswith('#'):
-                extras_require = [extra.strip() for extra in line.split(';')[1:]]
-                if not extras_require or any(extra in extras for extra in extras_require):
-                    requirements.append(line.split(';')[0])
-    return requirements
 
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='shuttleai', 
     version=version,
@@ -29,17 +19,22 @@
     package_dir={"": "src"},
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-    install_requires=read_requirements('requirements.txt'),
+    install_requires=[
+        'aiohttp',
+        'httpx',
+        'orjson',
+        'pydantic'
+    ],
     extras_require={
-        'cli': read_requirements('requirements.txt', extras=('cli',))
+        'cli': ['asyncclick', 'pystyle']
     },
     keywords=['shuttleai', 'ai', 'gpt', 'claude', 'api', 'free', 'chatgpt', 'gpt-4'],
     url='https://github.com/shuttleai/shuttleai-python',
     entry_points={
         'console_scripts': [
             'shuttleai = shuttleai.cli:main [cli]'
         ],
```

### Comparing `shuttleai-3.8.3/src/shuttleai/__init__.py` & `shuttleai-3.8.4/src/shuttleai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .client import ShuttleAsyncClient, ShuttleClient
 
 from sys import executable
 from os import system
 from httpx import get
 
-__version__ = "3.8.3"
+__version__ = "3.8.4"
 
 try:
     CURRENT_VERSION = get(
         "https://pypi.org/pypi/shuttleai/json").json().get("info").get("version")
 except:
     CURRENT_VERSION = __version__
```

### Comparing `shuttleai-3.8.3/src/shuttleai/cli.py` & `shuttleai-3.8.4/src/shuttleai/cli.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.3/src/shuttleai/client/_async.py` & `shuttleai-3.8.4/src/shuttleai/client/_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 @Author: ShuttleAI
-@Version: 3.8.3
+@Version: 3.8.4
 @Date: 4-5-2024
 """
 from __future__ import annotations
 from typing import (
     List,
     Dict,
     Any,
```

### Comparing `shuttleai-3.8.3/src/shuttleai/client/_sync.py` & `shuttleai-3.8.4/src/shuttleai/client/_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 @Author: ShuttleAI
-@Version: 3.8.3
+@Version: 3.8.4
 @Date: 4-5-2024
 """
 from typing import Any, Dict, List, Union, Optional, TYPE_CHECKING, Generator
 if TYPE_CHECKING:
     from httpx import Response
 
 from ..log import log
```

### Comparing `shuttleai-3.8.3/src/shuttleai/log.py` & `shuttleai-3.8.4/src/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.3/src/shuttleai/schemas/schemas.py` & `shuttleai-3.8.4/src/shuttleai/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.3/src/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.8.4/src/shuttleai.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.3
+Version: 3.8.4
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: httpx
 Requires-Dist: aiohttp
+Requires-Dist: httpx
 Requires-Dist: orjson
 Requires-Dist: pydantic
 Provides-Extra: cli
-Requires-Dist: httpx; extra == "cli"
-Requires-Dist: aiohttp; extra == "cli"
-Requires-Dist: orjson; extra == "cli"
-Requires-Dist: pydantic; extra == "cli"
+Requires-Dist: asyncclick; extra == "cli"
+Requires-Dist: pystyle; extra == "cli"
 
 # The official Python library for the ShuttleAI API
 Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
 
 > *PRs appreciated 🙂*
 # Installation
 ## ShuttleAI
```

