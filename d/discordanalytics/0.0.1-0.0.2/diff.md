# Comparing `tmp/discordanalytics-0.0.1.tar.gz` & `tmp/discordanalytics-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordanalytics-0.0.1.tar", last modified: Sat Apr  6 17:03:28 2024, max compression
+gzip compressed data, was "discordanalytics-0.0.2.tar", last modified: Sat Apr  6 18:30:20 2024, max compression
```

## Comparing `discordanalytics-0.0.1.tar` & `discordanalytics-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 17:03:28.726661 discordanalytics-0.0.1/
--rw-rw-rw-   0        0        0      363 2024-04-06 17:03:28.723680 discordanalytics-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      680 2024-04-06 16:58:50.000000 discordanalytics-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 17:03:28.678520 discordanalytics-0.0.1/discordanalytics/
--rw-rw-rw-   0        0        0      125 2024-04-06 13:21:34.000000 discordanalytics-0.0.1/discordanalytics/__init__.py
--rw-rw-rw-   0        0        0     7092 2024-04-06 16:53:26.000000 discordanalytics-0.0.1/discordanalytics/client.py
-drwxrwxrwx   0        0        0        0 2024-04-06 17:03:28.699661 discordanalytics-0.0.1/discordanalytics.egg-info/
--rw-rw-rw-   0        0        0      363 2024-04-06 17:03:28.000000 discordanalytics-0.0.1/discordanalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-04-06 17:03:28.000000 discordanalytics-0.0.1/discordanalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 17:03:28.000000 discordanalytics-0.0.1/discordanalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-06 17:03:28.000000 discordanalytics-0.0.1/discordanalytics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      473 2024-04-06 17:00:50.000000 discordanalytics-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 17:03:28.726661 discordanalytics-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 18:30:20.963501 discordanalytics-0.0.2/
+-rw-rw-rw-   0        0        0     1095 2024-04-06 18:05:32.000000 discordanalytics-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      386 2024-04-06 18:30:20.961501 discordanalytics-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      680 2024-04-06 16:58:50.000000 discordanalytics-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 18:30:20.895342 discordanalytics-0.0.2/discordanalytics/
+-rw-rw-rw-   0        0        0      125 2024-04-06 17:54:05.000000 discordanalytics-0.0.2/discordanalytics/__init__.py
+-rw-rw-rw-   0        0        0     7065 2024-04-06 17:13:40.000000 discordanalytics-0.0.2/discordanalytics/client.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:30:20.959501 discordanalytics-0.0.2/discordanalytics.egg-info/
+-rw-rw-rw-   0        0        0      386 2024-04-06 18:30:20.000000 discordanalytics-0.0.2/discordanalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-06 18:30:20.000000 discordanalytics-0.0.2/discordanalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 18:30:20.000000 discordanalytics-0.0.2/discordanalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-06 18:30:20.000000 discordanalytics-0.0.2/discordanalytics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      473 2024-04-06 18:29:40.000000 discordanalytics-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 18:30:20.963501 discordanalytics-0.0.2/setup.cfg
```

### Comparing `discordanalytics-0.0.1/README.md` & `discordanalytics-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `discordanalytics-0.0.1/discordanalytics/client.py` & `discordanalytics-0.0.2/discordanalytics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import asyncio
 from datetime import datetime
 import discord
 from discord.enums import InteractionType
 import requests
 import sys
 
-# from .__init__ import __version__
-
-__version__ = "0.0.1"
+from .__init__ import __version__
 
 class ApiEndpoints:
   BASE_URL = "https://discordanalytics.xyz/api"
   BOT_URL = f"{BASE_URL}/bots/:id"
   STATS_URL = f"{BASE_URL}/bots/:id/stats"
 
 class ErrorCodes:
```

