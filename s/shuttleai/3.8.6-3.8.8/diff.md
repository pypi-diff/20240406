# Comparing `tmp/shuttleai-3.8.6.tar.gz` & `tmp/shuttleai-3.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.8.6.tar", last modified: Fri Apr  5 22:44:39 2024, max compression
+gzip compressed data, was "shuttleai-3.8.8.tar", last modified: Fri Apr  5 23:24:18 2024, max compression
```

## Comparing `shuttleai-3.8.6.tar` & `shuttleai-3.8.8.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 22:44:39.034584 shuttleai-3.8.6/
--rw-rw-rw-   0        0        0     4116 2024-04-05 22:44:39.032065 shuttleai-3.8.6/PKG-INFO
--rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 22:44:39.035586 shuttleai-3.8.6/setup.cfg
--rw-rw-rw-   0        0        0     1328 2024-04-05 22:44:21.000000 shuttleai-3.8.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:44:38.952135 shuttleai-3.8.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 22:44:38.959267 shuttleai-3.8.6/src/shuttleai/
--rw-rw-rw-   0        0        0      576 2024-04-05 22:40:26.000000 shuttleai-3.8.6/src/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.6/src/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:44:39.021533 shuttleai-3.8.6/src/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.6/src/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17322 2024-04-05 22:37:02.000000 shuttleai-3.8.6/src/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0    15233 2024-04-05 22:36:13.000000 shuttleai-3.8.6/src/shuttleai/client/_sync.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.6/src/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:44:39.027066 shuttleai-3.8.6/src/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.6/src/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     4108 2024-04-05 22:32:01.000000 shuttleai-3.8.6/src/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:44:39.030065 shuttleai-3.8.6/src/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     4116 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 23:24:18.844355 shuttleai-3.8.8/
+-rw-rw-rw-   0        0        0     4116 2024-04-05 23:24:18.843357 shuttleai-3.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 23:24:18.844355 shuttleai-3.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     1274 2024-04-05 23:24:09.000000 shuttleai-3.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 23:24:18.814767 shuttleai-3.8.8/shuttleai/
+-rw-rw-rw-   0        0        0      578 2024-04-05 23:12:12.000000 shuttleai-3.8.8/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.8/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-05 23:24:18.836349 shuttleai-3.8.8/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.8/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17322 2024-04-05 22:37:02.000000 shuttleai-3.8.8/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0    15233 2024-04-05 22:36:13.000000 shuttleai-3.8.8/shuttleai/client/_sync.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.8/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-05 23:24:18.839357 shuttleai-3.8.8/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.8/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     4108 2024-04-05 22:32:01.000000 shuttleai-3.8.8/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-05 23:24:18.841356 shuttleai-3.8.8/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     4116 2024-04-05 23:24:18.000000 shuttleai-3.8.8/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2024-04-05 23:24:18.000000 shuttleai-3.8.8/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 23:24:18.000000 shuttleai-3.8.8/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 23:24:18.000000 shuttleai-3.8.8/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2024-04-05 23:24:18.000000 shuttleai-3.8.8/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 23:24:18.000000 shuttleai-3.8.8/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.8.6/PKG-INFO` & `shuttleai-3.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.6
+Version: 3.8.8
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shuttleai-3.8.6/README.md` & `shuttleai-3.8.8/README.md`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.6/setup.py` & `shuttleai-3.8.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-from src.shuttleai import __version__ as version
-
 
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 setup(
+    include_package_data=True,
     name='shuttleai', 
-    version=version,
+    version='3.8.8',
     author='shuttle',
     author_email='noreply@shuttleai.app',
     description="Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai",
     long_description_content_type='text/markdown',
     long_description=long_description,
-    packages=find_packages("src"),
-    package_dir={"": "src"},
+    packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.7',
     install_requires=[
         'aiohttp',
         'httpx',
         'orjson',
-        'python-dateutil'
+        'python-dateutil',
     ],
     extras_require={
         'cli': ['asyncclick', 'pystyle']
     },
     keywords=['shuttleai', 'ai', 'gpt', 'claude', 'api', 'free', 'chatgpt', 'gpt-4'],
     url='https://github.com/shuttleai/shuttleai-python',
     entry_points={
```

### Comparing `shuttleai-3.8.6/src/shuttleai/__init__.py` & `shuttleai-3.8.8/shuttleai/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+__version__ = "3.8.8"
+
 from .client import ShuttleAsyncClient, ShuttleClient
 
 from sys import executable
 from os import system
 from httpx import get
 
-__version__ = "3.8.6"
 
 try:
     CURRENT_VERSION = get(
         "https://pypi.org/pypi/shuttleai/json").json().get("info").get("version")
 except:
     CURRENT_VERSION = __version__
```

### Comparing `shuttleai-3.8.6/src/shuttleai/cli.py` & `shuttleai-3.8.8/shuttleai/cli.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.6/src/shuttleai/client/_async.py` & `shuttleai-3.8.8/shuttleai/client/_async.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.6/src/shuttleai/client/_sync.py` & `shuttleai-3.8.8/shuttleai/client/_sync.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.6/src/shuttleai/log.py` & `shuttleai-3.8.8/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.6/src/shuttleai/schemas/schemas.py` & `shuttleai-3.8.8/shuttleai/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.6/src/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.8.8/shuttleai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.6
+Version: 3.8.8
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

