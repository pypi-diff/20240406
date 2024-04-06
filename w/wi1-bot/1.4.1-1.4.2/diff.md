# Comparing `tmp/wi1-bot-1.4.1.tar.gz` & `tmp/wi1-bot-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wi1-bot-1.4.1.tar", last modified: Wed Oct 11 07:20:03 2023, max compression
+gzip compressed data, was "wi1-bot-1.4.2.tar", last modified: Sat Apr  6 01:31:31 2024, max compression
```

## Comparing `wi1-bot-1.4.1.tar` & `wi1-bot-1.4.2.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.971484 wi1-bot-1.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-11 07:20:03.979484 wi1-bot-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/tests/movie_downloaded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/wi1_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-11 07:20:03.000000 wi1-bot-1.4.1/wi1_bot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/wi1_bot/arr/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/arr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/arr/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/arr/episode.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/arr/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/arr/radarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/arr/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/wi1_bot/discord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/discord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/wi1_bot/discord/cogs/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/discord/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/discord/cogs/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/discord/cogs/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/discord/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/push.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/wi1_bot/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/scripts/add_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/scripts/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/scripts/transcode_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/wi1_bot/transcoder/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/transcoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/transcoder/transcode_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/transcoder/transcoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2023-10-11 07:19:49.000000 wi1-bot-1.4.1/wi1_bot/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:20:03.975484 wi1-bot-1.4.1/wi1_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2023-10-11 07:20:03.000000 wi1-bot-1.4.1/wi1_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-10-11 07:20:03.000000 wi1-bot-1.4.1/wi1_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 07:20:03.000000 wi1-bot-1.4.1/wi1_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-10-11 07:20:03.000000 wi1-bot-1.4.1/wi1_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2023-10-11 07:20:03.000000 wi1-bot-1.4.1/wi1_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-11 07:20:03.000000 wi1-bot-1.4.1/wi1_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.792701 wi1-bot-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.784701 wi1-bot-1.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.784701 wi1-bot-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.784701 wi1-bot-1.4.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-06 01:31:31.792701 wi1-bot-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 01:31:31.792701 wi1-bot-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.784701 wi1-bot-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/tests/movie_downloaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.788701 wi1-bot-1.4.2/wi1_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 01:31:30.000000 wi1-bot-1.4.2/wi1_bot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.788701 wi1-bot-1.4.2/wi1_bot/arr/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/arr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/arr/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/arr/episode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/arr/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/arr/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/arr/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.788701 wi1-bot-1.4.2/wi1_bot/discord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/discord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.788701 wi1-bot-1.4.2/wi1_bot/discord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/discord/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/discord/cogs/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/discord/cogs/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/discord/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/push.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.792701 wi1-bot-1.4.2/wi1_bot/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/scripts/add_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/scripts/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/scripts/transcode_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.792701 wi1-bot-1.4.2/wi1_bot/transcoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/transcoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/transcoder/transcode_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/transcoder/transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-06 01:31:23.000000 wi1-bot-1.4.2/wi1_bot/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:31:31.788701 wi1-bot-1.4.2/wi1_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-06 01:31:31.000000 wi1-bot-1.4.2/wi1_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-06 01:31:31.000000 wi1-bot-1.4.2/wi1_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 01:31:31.000000 wi1-bot-1.4.2/wi1_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-06 01:31:31.000000 wi1-bot-1.4.2/wi1_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-06 01:31:31.000000 wi1-bot-1.4.2/wi1_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 01:31:31.000000 wi1-bot-1.4.2/wi1_bot.egg-info/top_level.txt
```

### Comparing `wi1-bot-1.4.1/.github/workflows/pypi-publish.yml` & `wi1-bot-1.4.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/LICENSE` & `wi1-bot-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/PKG-INFO` & `wi1-bot-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.4.1
+Version: 1.4.2
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.4.1/README.md` & `wi1-bot-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/config.yaml.template` & `wi1-bot-1.4.2/config.yaml.template`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ---
 general:
   # log file directory, optional
   log_dir: /var/log/wi1-bot
+  # remote path mappings, optional
+  remote_path_mappings:
+    - remote: /data
+      local: /mnt/plex
 
 radarr:
   # radarr url you use to get to the dashboard
   url: http://localhost:7878
   # radarr api key (Settings->General->Security->API Key)
   api_key: XXX
   # radarr root folder (absolute path)
@@ -45,15 +49,14 @@
   # comma separated list of pushover device names
   devices: device1,device2
 
 # transcoding settings, optional
 transcoding:
   # -hwaccel in ffmpeg, optional
   hwaccel: cuda
-  
   profiles:
     # name of profile must match name in radarr/sonarr
     good:
       # copy all video and audio streams
       copy_all_streams: false
       # comma separated ISO 639-2 codes, optional
       # currently only applies to choosing which subtitle streams to copy
```

### Comparing `wi1-bot-1.4.1/pyproject.toml` & `wi1-bot-1.4.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,55 @@
-[build-system]
-requires = ["setuptools==61.*", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
-
 [project]
 name = "wi1-bot"
 description = "Discord bot for Radarr/Sonarr integration"
 authors = [{ name = "William Huebner", email = "wilhueb@gmail.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10"
 ]
 dynamic = ["version"]
 requires-python = ">=3.10"
 dependencies = [
-    "discord.py==2.3.1",
-    "Flask==2.3.2",
-    "mongoengine==0.27.0",
+    "discord.py==2.3.2",
+    "Flask==3.0.2",
+    "mongoengine==0.28.0",
     "pyarr==5.2.0",
     "PyYAML==6.0.1",
     "requests==2.31.0"
 ]
 
-[project.optional-dependencies]
-dev = [
-    "black==23.3.0",
-    "flake8==6.0.0",
-    "isort==5.12.0",
-    "mongo-types==0.15.1",
-    "mypy==1.2.0",
-    "pre-commit==3.2.2",
-    "types-PyYAML==6.0.12.9",
-]
-
 [project.urls]
 Homepage = "https://github.com/wthueb/wi1-bot"
 
 [project.scripts]
 wi1-bot = "wi1_bot.scripts.start:main"
 transcode-item = "wi1_bot.scripts.transcode_item:main"
 add-tag = "wi1_bot.scripts.add_tag:main"
 
+[project.optional-dependencies]
+dev = [
+    "mongo-types==0.15.1",
+    "mypy==1.3.0",
+    "pre-commit==3.6.2",
+    "ruff==0.3.0",
+    "types-PyYAML==6.0.12.12",
+]
+
+[build-system]
+requires = ["setuptools==61.*", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
 [tool.setuptools]
 packages = ["wi1_bot"]
 
 [tool.setuptools_scm]
 write_to = "wi1_bot/_version.py"
 
+[tool.ruff.lint]
+select = ["E", "F", "I"]
+
 [tool.mypy]
 packages = "wi1_bot"
 strict = true
-
-[[tool.mypy.overrides]]
-module = [
-    "pushover",
-    "pyarr",
-]
-ignore_missing_imports = true
-
-[tool.black]
-line-length = 88
-target-version = ["py310"]
-
-[tool.isort]
-profile = "black"
-known_first_party = ["wi1_bot"]
```

### Comparing `wi1-bot-1.4.1/wi1_bot/arr/download.py` & `wi1-bot-1.4.2/wi1_bot/arr/download.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/arr/episode.py` & `wi1-bot-1.4.2/wi1_bot/arr/episode.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/arr/movie.py` & `wi1-bot-1.4.2/wi1_bot/arr/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/arr/radarr.py` & `wi1-bot-1.4.2/wi1_bot/arr/radarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/arr/sonarr.py` & `wi1-bot-1.4.2/wi1_bot/arr/sonarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/config.py` & `wi1-bot-1.4.2/wi1_bot/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -95,16 +95,22 @@
     hwaccel: str  # optional
 
 
 class TranscodingConfig(TranscodingConfigOptional):
     profiles: dict[str, TranscodingProfile]
 
 
+class RemotePathMapping(TypedDict):
+    remote: str
+    local: str
+
+
 class GeneralConfigOptional(TypedDict, total=False):
     log_dir: str
+    remote_path_mappings: list[RemotePathMapping]
 
 
 class GeneralConfig(GeneralConfigOptional):
     pass
 
 
 class ConfigOptional(TypedDict, total=False):
```

### Comparing `wi1-bot-1.4.1/wi1_bot/discord/bot.py` & `wi1-bot-1.4.2/wi1_bot/discord/bot.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/discord/cogs/movie.py` & `wi1-bot-1.4.2/wi1_bot/discord/cogs/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/discord/cogs/series.py` & `wi1-bot-1.4.2/wi1_bot/discord/cogs/series.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/discord/helpers.py` & `wi1-bot-1.4.2/wi1_bot/discord/helpers.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/push.py` & `wi1-bot-1.4.2/wi1_bot/push.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/scripts/add_tag.py` & `wi1-bot-1.4.2/wi1_bot/scripts/add_tag.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/scripts/start.py` & `wi1-bot-1.4.2/wi1_bot/scripts/start.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/scripts/transcode_item.py` & `wi1-bot-1.4.2/wi1_bot/scripts/transcode_item.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/transcoder/transcode_queue.py` & `wi1-bot-1.4.2/wi1_bot/transcoder/transcode_queue.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot/transcoder/transcoder.py` & `wi1-bot-1.4.2/wi1_bot/transcoder/transcoder.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.1/wi1_bot.egg-info/PKG-INFO` & `wi1-bot-1.4.2/wi1_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.4.1
+Version: 1.4.2
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.4.1/wi1_bot.egg-info/SOURCES.txt` & `wi1-bot-1.4.2/wi1_bot.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.flake8
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 config.yaml.template
 pyproject.toml
 setup.cfg
```

