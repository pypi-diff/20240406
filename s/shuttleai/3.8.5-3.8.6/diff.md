# Comparing `tmp/shuttleai-3.8.5.tar.gz` & `tmp/shuttleai-3.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.8.5.tar", last modified: Fri Apr  5 22:38:02 2024, max compression
+gzip compressed data, was "shuttleai-3.8.6.tar", last modified: Fri Apr  5 22:44:39 2024, max compression
```

## Comparing `shuttleai-3.8.5.tar` & `shuttleai-3.8.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.888396 shuttleai-3.8.5/
--rw-rw-rw-   0        0        0     4084 2024-04-05 22:38:02.885383 shuttleai-3.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 22:38:02.888396 shuttleai-3.8.5/setup.cfg
--rw-rw-rw-   0        0        0     1300 2024-04-05 22:37:34.000000 shuttleai-3.8.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.800159 shuttleai-3.8.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.806681 shuttleai-3.8.5/src/shuttleai/
--rw-rw-rw-   0        0        0      576 2024-04-05 22:37:41.000000 shuttleai-3.8.5/src/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.5/src/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.877868 shuttleai-3.8.5/src/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.5/src/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17322 2024-04-05 22:37:02.000000 shuttleai-3.8.5/src/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0    15233 2024-04-05 22:36:13.000000 shuttleai-3.8.5/src/shuttleai/client/_sync.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.5/src/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.880866 shuttleai-3.8.5/src/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.5/src/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     4108 2024-04-05 22:32:01.000000 shuttleai-3.8.5/src/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.882865 shuttleai-3.8.5/src/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     4084 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 22:44:39.034584 shuttleai-3.8.6/
+-rw-rw-rw-   0        0        0     4116 2024-04-05 22:44:39.032065 shuttleai-3.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 22:44:39.035586 shuttleai-3.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2024-04-05 22:44:21.000000 shuttleai-3.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:44:38.952135 shuttleai-3.8.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 22:44:38.959267 shuttleai-3.8.6/src/shuttleai/
+-rw-rw-rw-   0        0        0      576 2024-04-05 22:40:26.000000 shuttleai-3.8.6/src/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.6/src/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:44:39.021533 shuttleai-3.8.6/src/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.6/src/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17322 2024-04-05 22:37:02.000000 shuttleai-3.8.6/src/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0    15233 2024-04-05 22:36:13.000000 shuttleai-3.8.6/src/shuttleai/client/_sync.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.6/src/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:44:39.027066 shuttleai-3.8.6/src/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.6/src/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     4108 2024-04-05 22:32:01.000000 shuttleai-3.8.6/src/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:44:39.030065 shuttleai-3.8.6/src/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     4116 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 22:44:38.000000 shuttleai-3.8.6/src/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.8.5/PKG-INFO` & `shuttleai-3.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.5
+Version: 3.8.6
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: httpx
 Requires-Dist: orjson
+Requires-Dist: python-dateutil
 Provides-Extra: cli
 Requires-Dist: asyncclick; extra == "cli"
 Requires-Dist: pystyle; extra == "cli"
 
 # The official Python library for the ShuttleAI API
 Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
```

### Comparing `shuttleai-3.8.5/README.md` & `shuttleai-3.8.6/README.md`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.5/setup.py` & `shuttleai-3.8.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.7',
     install_requires=[
         'aiohttp',
         'httpx',
-        'orjson'
+        'orjson',
+        'python-dateutil'
     ],
     extras_require={
         'cli': ['asyncclick', 'pystyle']
     },
     keywords=['shuttleai', 'ai', 'gpt', 'claude', 'api', 'free', 'chatgpt', 'gpt-4'],
     url='https://github.com/shuttleai/shuttleai-python',
     entry_points={
```

### Comparing `shuttleai-3.8.5/src/shuttleai/__init__.py` & `shuttleai-3.8.6/src/shuttleai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .client import ShuttleAsyncClient, ShuttleClient
 
 from sys import executable
 from os import system
 from httpx import get
 
-__version__ = "3.8.5"
+__version__ = "3.8.6"
 
 try:
     CURRENT_VERSION = get(
         "https://pypi.org/pypi/shuttleai/json").json().get("info").get("version")
 except:
     CURRENT_VERSION = __version__
```

### Comparing `shuttleai-3.8.5/src/shuttleai/cli.py` & `shuttleai-3.8.6/src/shuttleai/cli.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.5/src/shuttleai/client/_async.py` & `shuttleai-3.8.6/src/shuttleai/client/_async.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.5/src/shuttleai/client/_sync.py` & `shuttleai-3.8.6/src/shuttleai/client/_sync.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.5/src/shuttleai/log.py` & `shuttleai-3.8.6/src/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.5/src/shuttleai/schemas/schemas.py` & `shuttleai-3.8.6/src/shuttleai/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.5/src/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.8.6/src/shuttleai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.5
+Version: 3.8.6
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: httpx
 Requires-Dist: orjson
+Requires-Dist: python-dateutil
 Provides-Extra: cli
 Requires-Dist: asyncclick; extra == "cli"
 Requires-Dist: pystyle; extra == "cli"
 
 # The official Python library for the ShuttleAI API
 Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
```

