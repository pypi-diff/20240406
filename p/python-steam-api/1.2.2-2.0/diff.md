# Comparing `tmp/python-steam-api-1.2.2.tar.gz` & `tmp/python-steam-api-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-steam-api-1.2.2.tar", last modified: Sat Dec 23 14:54:13 2023, max compression
+gzip compressed data, was "python-steam-api-2.0.tar", last modified: Sat Apr  6 16:13:06 2024, max compression
```

## Comparing `python-steam-api-1.2.2.tar` & `python-steam-api-2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 the12thchairman   (501) staff       (20)        0 2023-12-23 14:54:13.326632 python-steam-api-1.2.2/
--rw-r--r--   0 the12thchairman   (501) staff       (20)     1101 2023-08-22 00:13:40.000000 python-steam-api-1.2.2/LICENCE
--rw-r--r--   0 the12thchairman   (501) staff       (20)       48 2023-08-22 00:13:40.000000 python-steam-api-1.2.2/MANIFEST.in
--rw-r--r--   0 the12thchairman   (501) staff       (20)    18289 2023-12-23 14:54:13.326460 python-steam-api-1.2.2/PKG-INFO
--rw-r--r--   0 the12thchairman   (501) staff       (20)    17945 2023-09-02 15:14:38.000000 python-steam-api-1.2.2/README.md
-drwxr-xr-x   0 the12thchairman   (501) staff       (20)        0 2023-12-23 14:54:13.326244 python-steam-api-1.2.2/python_steam_api.egg-info/
--rw-r--r--   0 the12thchairman   (501) staff       (20)    18289 2023-12-23 14:54:13.000000 python-steam-api-1.2.2/python_steam_api.egg-info/PKG-INFO
--rw-r--r--   0 the12thchairman   (501) staff       (20)      367 2023-12-23 14:54:13.000000 python-steam-api-1.2.2/python_steam_api.egg-info/SOURCES.txt
--rw-r--r--   0 the12thchairman   (501) staff       (20)        1 2023-12-23 14:54:13.000000 python-steam-api-1.2.2/python_steam_api.egg-info/dependency_links.txt
--rw-r--r--   0 the12thchairman   (501) staff       (20)       25 2023-12-23 14:54:13.000000 python-steam-api-1.2.2/python_steam_api.egg-info/requires.txt
--rw-r--r--   0 the12thchairman   (501) staff       (20)        6 2023-12-23 14:54:13.000000 python-steam-api-1.2.2/python_steam_api.egg-info/top_level.txt
--rw-r--r--   0 the12thchairman   (501) staff       (20)       70 2023-12-23 14:54:13.326822 python-steam-api-1.2.2/setup.cfg
--rw-r--r--   0 the12thchairman   (501) staff       (20)     1184 2023-12-23 14:53:59.000000 python-steam-api-1.2.2/setup.py
-drwxr-xr-x   0 the12thchairman   (501) staff       (20)        0 2023-12-23 14:54:13.326087 python-steam-api-1.2.2/steam/
--rw-r--r--   0 the12thchairman   (501) staff       (20)      127 2023-08-22 00:13:40.000000 python-steam-api-1.2.2/steam/__init__.py
--rw-r--r--   0 the12thchairman   (501) staff       (20)     5776 2023-12-23 14:20:40.000000 python-steam-api-1.2.2/steam/apps.py
--rw-r--r--   0 the12thchairman   (501) staff       (20)     1821 2023-09-02 14:28:24.000000 python-steam-api-1.2.2/steam/client.py
--rw-r--r--   0 the12thchairman   (501) staff       (20)      188 2023-08-22 00:13:40.000000 python-steam-api-1.2.2/steam/constants.py
--rw-r--r--   0 the12thchairman   (501) staff       (20)      479 2023-09-02 14:28:03.000000 python-steam-api-1.2.2/steam/steam.py
--rw-r--r--   0 the12thchairman   (501) staff       (20)     5965 2023-09-02 14:27:55.000000 python-steam-api-1.2.2/steam/users.py
--rw-r--r--   0 the12thchairman   (501) staff       (20)     2180 2023-08-22 00:13:40.000000 python-steam-api-1.2.2/steam/utils.py
--rw-r--r--   0 the12thchairman   (501) staff       (20)      242 2023-12-23 14:37:50.000000 python-steam-api-1.2.2/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:13:06.370955 python-steam-api-2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-06 16:12:46.000000 python-steam-api-2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-06 16:13:06.370955 python-steam-api-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18235 2024-04-06 16:12:46.000000 python-steam-api-2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-06 16:12:46.000000 python-steam-api-2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:13:06.370955 python-steam-api-2.0/python_steam_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-06 16:13:06.000000 python-steam-api-2.0/python_steam_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 16:13:06.000000 python-steam-api-2.0/python_steam_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:13:06.000000 python-steam-api-2.0/python_steam_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-06 16:13:06.000000 python-steam-api-2.0/python_steam_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 16:13:06.000000 python-steam-api-2.0/python_steam_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:13:06.370955 python-steam-api-2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:13:06.366955 python-steam-api-2.0/steam_web_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/utils.py
```

### Comparing `python-steam-api-1.2.2/LICENCE` & `python-steam-api-2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `python-steam-api-1.2.2/PKG-INFO` & `python-steam-api-2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,70 @@
 Metadata-Version: 2.1
 Name: python-steam-api
-Version: 1.2.2
-Summary: Python Client wrapper for Steam API
-Home-page: https://github.com/deivit24/steam-python-sdk
-Author: David Salazar
-Author-email: david.asal@hotmail.com
-License: MIT
-Keywords: steam,steamapi,steam community,api
+Version: 2.0
+Summary: Python Client wrapper for Steam API.
+Author-email: David Salazar <david.asal@hotmail.com>
+Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
+Project-URL: source, https://github.com/deivit24/python-steam-api
+Project-URL: tracker, https://github.com/deivit24/python-steam-api/issues
+Keywords: api,python,steam community,steam,steamapi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE
+Requires-Dist: beautifulsoup4
 Requires-Dist: requests
-Requires-Dist: python-decouple
+Provides-Extra: all
+Requires-Dist: python-steam-api[build]; extra == "all"
+Requires-Dist: python-steam-api[style]; extra == "all"
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Requires-Dist: twine; extra == "build"
+Provides-Extra: full
+Requires-Dist: python-steam-api[all]; extra == "full"
+Provides-Extra: style
+Requires-Dist: codespell[toml]>=2.2.4; extra == "style"
+Requires-Dist: isort; extra == "style"
+Requires-Dist: ruff>=0.1.8; extra == "style"
+Requires-Dist: toml-sort; extra == "style"
+Requires-Dist: yamllint; extra == "style"
 
 # Get Started
 
 ## Installation
 
 `pip install python-steam-api`
 
-## Pip install requirements
-
-`pip install beautifulsoup4`
-
 ## Create Steam API web key
 
 [Steam API Web key](https://steamcommunity.com/dev/apikey)
 
 Follow instructions to get API Key
 
-## Create .env file
-
-From root of your project
+# Set up your environment variable
 
-`touch .env`
-
-`echo "STEAM_API_KEY=<YOUR_STEAM_API KEY>" >> .env`
+To create an environment variable in Python, you can utilize the os module. Use os.environ to access and modify environment variables. To accommodate different operating systems, check the documentation or resources specific to each OS for instructions on setting environment variables. For example, on Windows, you can use the Command Prompt or PowerShell, while on Unix-based systems like Linux or macOS, you can modify configuration files or use terminal commands like export.
 
 # Basic Usage
 
 ### Searching for a user
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 steam = Steam(KEY)
 
 steam.users.search_user("the12thchairman")
 ```
 
 Response
 
@@ -82,18 +89,18 @@
   }
 }
 ```
 
 ### Getting User details by steam id
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_details("76561198995017863")
 ```
 
@@ -120,18 +127,18 @@
   }
 }
 ```
 
 ### Getting Friends List
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_friends_list("76561198995017863")
 ```
@@ -202,108 +209,102 @@
   ]
 }
 ```
 
 ### Getting Users Recently Played Games
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_recently_played_games("76561198995017863")
 ```
 
 ### Getting User Owned Games
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam()
 
 # arguments: steamid
 user = steam.users.get_owned_games("76561198995017863")
 ```
 
 ### Getting User Steam Level
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_steam_level("76561198995017863")
 ```
 
 ### Getting User Badges
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_badges("76561198995017863")
 ```
 
 ### Getting Community Badge Progress
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid, badgeid
 user = steam.users.get_community_badge_progress("<steam_id>", "<badge_id>")
 ```
 
 ### Getting User Public Account
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_account_public_info("<steam_id>")
 ```
 
 ### Searching for Games
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: search
 user = steam.apps.search_games("terr")
 ```
@@ -353,15 +354,15 @@
 ```
 
 ### App/Game details
 
 #### Parameters:
 
 - `app_id` (int): The unique App ID of the app you want to retrieve details for. For example, 105600 corresponds to "Terraria"
-
+  i
 - `country` (str): An optional parameter representing the ISO Country Code. The default value is "US."
 
 - `filters` (str): An optional parameter that allows you to specify a list of keys to return in the app details. If not provided, it defaults to "basic." The available filter options include:
 
 - `basic` (Default): Returns essential information like type, name, steam_appid, required_age, is_free, dlc, detailed_description, short_description, about_the_game, supported_languages, header_image, website, pc_requirements, mac_requirements, and linux_requirements.
 
 - Optional filters (Specify one or more of these as a comma-separated string):
@@ -375,22 +376,21 @@
   - metacritic
   - categories
   - genres
   - screenshots
   - movies
   - recommendations
   - achievements
-Response
+    Response
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 terraria_app_id = 105600
 steam = Steam(KEY)
 
 # arguments: app_id
 user = steam.apps.get_app_details(terraria_app_id)
 
@@ -403,18 +403,15 @@
     "data": {
       "type": "game",
       "name": "Terraria",
       "steam_appid": 105600,
       "required_age": 0,
       "is_free": false,
       "controller_support": "full",
-      "dlc": [
-      409210,
-      1323320
-      ],
+      "dlc": [409210, 1323320],
       "detailed_description": "Dig, Fight, Explore, Build:  The very world is at your fingertips as you fight for survival, fortune, and glory.   Will you delve deep into cavernous expanses in search of treasure and raw materials with which to craft ever-evolving gear, machinery, and aesthetics?   Perhaps you will choose instead to seek out ever-greater foes to test your mettle in combat?   Maybe you will decide to construct your own city to house the host of mysterious allies you may encounter along your travels? <br><br>In the World of Terraria, the choice is yours!<br><br>Blending elements of classic action games with the freedom of sandbox-style creativity, Terraria is a unique gaming experience where both the journey and the destination are completely in the player’s control.   The Terraria adventure is truly as unique as the players themselves!  <br><br>Are you up for the monumental task of exploring, creating, and defending a world of your own?  <br><br>\t\t\t\t\t\t\t<strong>Key features:</strong><br>\t\t\t\t\t\t\t<ul class=\"bb_ul\"><li>Sandbox Play<br>\t\t\t\t\t\t\t</li><li> Randomly generated worlds<br>\t\t\t\t\t\t\t</li><li>Free Content Updates<br>\t\t\t\t\t\t\t</li></ul>",
       "about_the_game": "Dig, Fight, Explore, Build:  The very world is at your fingertips as you fight for survival, fortune, and glory.   Will you delve deep into cavernous expanses in search of treasure and raw materials with which to craft ever-evolving gear, machinery, and aesthetics?   Perhaps you will choose instead to seek out ever-greater foes to test your mettle in combat?   Maybe you will decide to construct your own city to house the host of mysterious allies you may encounter along your travels? <br><br>In the World of Terraria, the choice is yours!<br><br>Blending elements of classic action games with the freedom of sandbox-style creativity, Terraria is a unique gaming experience where both the journey and the destination are completely in the player’s control.   The Terraria adventure is truly as unique as the players themselves!  <br><br>Are you up for the monumental task of exploring, creating, and defending a world of your own?  <br><br>\t\t\t\t\t\t\t<strong>Key features:</strong><br>\t\t\t\t\t\t\t<ul class=\"bb_ul\"><li>Sandbox Play<br>\t\t\t\t\t\t\t</li><li> Randomly generated worlds<br>\t\t\t\t\t\t\t</li><li>Free Content Updates<br>\t\t\t\t\t\t\t</li></ul>",
       "short_description": "Dig, fight, explore, build! Nothing is impossible in this action-packed adventure game. Four Pack also available!",
       "supported_languages": "English, French, Italian, German, Spanish - Spain, Polish, Portuguese - Brazil, Russian, Simplified Chinese",
       "header_image": "https://cdn.akamai.steamstatic.com/steam/apps/105600/header.jpg?t=1666290860",
       "capsule_image": "https://cdn.akamai.steamstatic.com/steam/apps/105600/capsule_231x87.jpg?t=1666290860",
       "capsule_imagev5": "https://cdn.akamai.steamstatic.com/steam/apps/105600/capsule_184x69.jpg?t=1666290860",
@@ -435,67 +432,63 @@
   }
 }
 ```
 
 ### Getting user app stats
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steam_id, app_id
 user = steam.apps.get_user_stats("<steam_id>", "<app_id>")
 ```
 
 ### Getting user app achievements
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: steam_id, app_id
 user = steam.apps.get_user_achievements("<steam_id>", "<app_id>")
 ```
 
-
 ### Getting user ban status
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: steam_id
 user = steam.users.get_player_bans("<steam_id>")
-````
-
+```
 
 ```json
 {
-"players":[
+  "players": [
     {
-    "SteamId":"76561198079362196",
-    "CommunityBanned":false,
-    "VACBanned":false,
-    "NumberOfVACBans":0,
-    "DaysSinceLastBan":0,
-    "NumberOfGameBans":0,
-    "EconomyBan":"none"
+      "SteamId": "76561198079362196",
+      "CommunityBanned": false,
+      "VACBanned": false,
+      "NumberOfVACBans": 0,
+      "DaysSinceLastBan": 0,
+      "NumberOfGameBans": 0,
+      "EconomyBan": "none"
     }
-    ]
+  ]
 }
 ```
-
```

### Comparing `python-steam-api-1.2.2/README.md` & `python-steam-api-2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 # Get Started
 
 ## Installation
 
 `pip install python-steam-api`
 
-## Pip install requirements
-
-`pip install beautifulsoup4`
-
 ## Create Steam API web key
 
 [Steam API Web key](https://steamcommunity.com/dev/apikey)
 
 Follow instructions to get API Key
 
-## Create .env file
-
-From root of your project
+# Set up your environment variable
 
-`touch .env`
-
-`echo "STEAM_API_KEY=<YOUR_STEAM_API KEY>" >> .env`
+To create an environment variable in Python, you can utilize the os module. Use os.environ to access and modify environment variables. To accommodate different operating systems, check the documentation or resources specific to each OS for instructions on setting environment variables. For example, on Windows, you can use the Command Prompt or PowerShell, while on Unix-based systems like Linux or macOS, you can modify configuration files or use terminal commands like export.
 
 # Basic Usage
 
 ### Searching for a user
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 steam = Steam(KEY)
 
 steam.users.search_user("the12thchairman")
 ```
 
 Response
 
@@ -59,18 +51,18 @@
   }
 }
 ```
 
 ### Getting User details by steam id
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_details("76561198995017863")
 ```
 
@@ -97,18 +89,18 @@
   }
 }
 ```
 
 ### Getting Friends List
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_friends_list("76561198995017863")
 ```
@@ -179,108 +171,102 @@
   ]
 }
 ```
 
 ### Getting Users Recently Played Games
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_recently_played_games("76561198995017863")
 ```
 
 ### Getting User Owned Games
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam()
 
 # arguments: steamid
 user = steam.users.get_owned_games("76561198995017863")
 ```
 
 ### Getting User Steam Level
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_steam_level("76561198995017863")
 ```
 
 ### Getting User Badges
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_badges("76561198995017863")
 ```
 
 ### Getting Community Badge Progress
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid, badgeid
 user = steam.users.get_community_badge_progress("<steam_id>", "<badge_id>")
 ```
 
 ### Getting User Public Account
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_account_public_info("<steam_id>")
 ```
 
 ### Searching for Games
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: search
 user = steam.apps.search_games("terr")
 ```
@@ -330,15 +316,15 @@
 ```
 
 ### App/Game details
 
 #### Parameters:
 
 - `app_id` (int): The unique App ID of the app you want to retrieve details for. For example, 105600 corresponds to "Terraria"
-
+  i
 - `country` (str): An optional parameter representing the ISO Country Code. The default value is "US."
 
 - `filters` (str): An optional parameter that allows you to specify a list of keys to return in the app details. If not provided, it defaults to "basic." The available filter options include:
 
 - `basic` (Default): Returns essential information like type, name, steam_appid, required_age, is_free, dlc, detailed_description, short_description, about_the_game, supported_languages, header_image, website, pc_requirements, mac_requirements, and linux_requirements.
 
 - Optional filters (Specify one or more of these as a comma-separated string):
@@ -352,22 +338,21 @@
   - metacritic
   - categories
   - genres
   - screenshots
   - movies
   - recommendations
   - achievements
-Response
+    Response
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 terraria_app_id = 105600
 steam = Steam(KEY)
 
 # arguments: app_id
 user = steam.apps.get_app_details(terraria_app_id)
 
@@ -380,18 +365,15 @@
     "data": {
       "type": "game",
       "name": "Terraria",
       "steam_appid": 105600,
       "required_age": 0,
       "is_free": false,
       "controller_support": "full",
-      "dlc": [
-      409210,
-      1323320
-      ],
+      "dlc": [409210, 1323320],
       "detailed_description": "Dig, Fight, Explore, Build:  The very world is at your fingertips as you fight for survival, fortune, and glory.   Will you delve deep into cavernous expanses in search of treasure and raw materials with which to craft ever-evolving gear, machinery, and aesthetics?   Perhaps you will choose instead to seek out ever-greater foes to test your mettle in combat?   Maybe you will decide to construct your own city to house the host of mysterious allies you may encounter along your travels? <br><br>In the World of Terraria, the choice is yours!<br><br>Blending elements of classic action games with the freedom of sandbox-style creativity, Terraria is a unique gaming experience where both the journey and the destination are completely in the player’s control.   The Terraria adventure is truly as unique as the players themselves!  <br><br>Are you up for the monumental task of exploring, creating, and defending a world of your own?  <br><br>\t\t\t\t\t\t\t<strong>Key features:</strong><br>\t\t\t\t\t\t\t<ul class=\"bb_ul\"><li>Sandbox Play<br>\t\t\t\t\t\t\t</li><li> Randomly generated worlds<br>\t\t\t\t\t\t\t</li><li>Free Content Updates<br>\t\t\t\t\t\t\t</li></ul>",
       "about_the_game": "Dig, Fight, Explore, Build:  The very world is at your fingertips as you fight for survival, fortune, and glory.   Will you delve deep into cavernous expanses in search of treasure and raw materials with which to craft ever-evolving gear, machinery, and aesthetics?   Perhaps you will choose instead to seek out ever-greater foes to test your mettle in combat?   Maybe you will decide to construct your own city to house the host of mysterious allies you may encounter along your travels? <br><br>In the World of Terraria, the choice is yours!<br><br>Blending elements of classic action games with the freedom of sandbox-style creativity, Terraria is a unique gaming experience where both the journey and the destination are completely in the player’s control.   The Terraria adventure is truly as unique as the players themselves!  <br><br>Are you up for the monumental task of exploring, creating, and defending a world of your own?  <br><br>\t\t\t\t\t\t\t<strong>Key features:</strong><br>\t\t\t\t\t\t\t<ul class=\"bb_ul\"><li>Sandbox Play<br>\t\t\t\t\t\t\t</li><li> Randomly generated worlds<br>\t\t\t\t\t\t\t</li><li>Free Content Updates<br>\t\t\t\t\t\t\t</li></ul>",
       "short_description": "Dig, fight, explore, build! Nothing is impossible in this action-packed adventure game. Four Pack also available!",
       "supported_languages": "English, French, Italian, German, Spanish - Spain, Polish, Portuguese - Brazil, Russian, Simplified Chinese",
       "header_image": "https://cdn.akamai.steamstatic.com/steam/apps/105600/header.jpg?t=1666290860",
       "capsule_image": "https://cdn.akamai.steamstatic.com/steam/apps/105600/capsule_231x87.jpg?t=1666290860",
       "capsule_imagev5": "https://cdn.akamai.steamstatic.com/steam/apps/105600/capsule_184x69.jpg?t=1666290860",
@@ -412,67 +394,63 @@
   }
 }
 ```
 
 ### Getting user app stats
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steam_id, app_id
 user = steam.apps.get_user_stats("<steam_id>", "<app_id>")
 ```
 
 ### Getting user app achievements
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: steam_id, app_id
 user = steam.apps.get_user_achievements("<steam_id>", "<app_id>")
 ```
 
-
 ### Getting user ban status
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: steam_id
 user = steam.users.get_player_bans("<steam_id>")
-````
-
+```
 
 ```json
 {
-"players":[
+  "players": [
     {
-    "SteamId":"76561198079362196",
-    "CommunityBanned":false,
-    "VACBanned":false,
-    "NumberOfVACBans":0,
-    "DaysSinceLastBan":0,
-    "NumberOfGameBans":0,
-    "EconomyBan":"none"
+      "SteamId": "76561198079362196",
+      "CommunityBanned": false,
+      "VACBanned": false,
+      "NumberOfVACBans": 0,
+      "DaysSinceLastBan": 0,
+      "NumberOfGameBans": 0,
+      "EconomyBan": "none"
     }
-    ]
+  ]
 }
 ```
-
```

### Comparing `python-steam-api-1.2.2/python_steam_api.egg-info/PKG-INFO` & `python-steam-api-2.0/python_steam_api.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,70 @@
 Metadata-Version: 2.1
 Name: python-steam-api
-Version: 1.2.2
-Summary: Python Client wrapper for Steam API
-Home-page: https://github.com/deivit24/steam-python-sdk
-Author: David Salazar
-Author-email: david.asal@hotmail.com
-License: MIT
-Keywords: steam,steamapi,steam community,api
+Version: 2.0
+Summary: Python Client wrapper for Steam API.
+Author-email: David Salazar <david.asal@hotmail.com>
+Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
+Project-URL: source, https://github.com/deivit24/python-steam-api
+Project-URL: tracker, https://github.com/deivit24/python-steam-api/issues
+Keywords: api,python,steam community,steam,steamapi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE
+Requires-Dist: beautifulsoup4
 Requires-Dist: requests
-Requires-Dist: python-decouple
+Provides-Extra: all
+Requires-Dist: python-steam-api[build]; extra == "all"
+Requires-Dist: python-steam-api[style]; extra == "all"
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Requires-Dist: twine; extra == "build"
+Provides-Extra: full
+Requires-Dist: python-steam-api[all]; extra == "full"
+Provides-Extra: style
+Requires-Dist: codespell[toml]>=2.2.4; extra == "style"
+Requires-Dist: isort; extra == "style"
+Requires-Dist: ruff>=0.1.8; extra == "style"
+Requires-Dist: toml-sort; extra == "style"
+Requires-Dist: yamllint; extra == "style"
 
 # Get Started
 
 ## Installation
 
 `pip install python-steam-api`
 
-## Pip install requirements
-
-`pip install beautifulsoup4`
-
 ## Create Steam API web key
 
 [Steam API Web key](https://steamcommunity.com/dev/apikey)
 
 Follow instructions to get API Key
 
-## Create .env file
-
-From root of your project
+# Set up your environment variable
 
-`touch .env`
-
-`echo "STEAM_API_KEY=<YOUR_STEAM_API KEY>" >> .env`
+To create an environment variable in Python, you can utilize the os module. Use os.environ to access and modify environment variables. To accommodate different operating systems, check the documentation or resources specific to each OS for instructions on setting environment variables. For example, on Windows, you can use the Command Prompt or PowerShell, while on Unix-based systems like Linux or macOS, you can modify configuration files or use terminal commands like export.
 
 # Basic Usage
 
 ### Searching for a user
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 steam = Steam(KEY)
 
 steam.users.search_user("the12thchairman")
 ```
 
 Response
 
@@ -82,18 +89,18 @@
   }
 }
 ```
 
 ### Getting User details by steam id
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_details("76561198995017863")
 ```
 
@@ -120,18 +127,18 @@
   }
 }
 ```
 
 ### Getting Friends List
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_friends_list("76561198995017863")
 ```
@@ -202,108 +209,102 @@
   ]
 }
 ```
 
 ### Getting Users Recently Played Games
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_recently_played_games("76561198995017863")
 ```
 
 ### Getting User Owned Games
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam()
 
 # arguments: steamid
 user = steam.users.get_owned_games("76561198995017863")
 ```
 
 ### Getting User Steam Level
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_steam_level("76561198995017863")
 ```
 
 ### Getting User Badges
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_user_badges("76561198995017863")
 ```
 
 ### Getting Community Badge Progress
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid, badgeid
 user = steam.users.get_community_badge_progress("<steam_id>", "<badge_id>")
 ```
 
 ### Getting User Public Account
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steamid
 user = steam.users.get_account_public_info("<steam_id>")
 ```
 
 ### Searching for Games
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: search
 user = steam.apps.search_games("terr")
 ```
@@ -353,15 +354,15 @@
 ```
 
 ### App/Game details
 
 #### Parameters:
 
 - `app_id` (int): The unique App ID of the app you want to retrieve details for. For example, 105600 corresponds to "Terraria"
-
+  i
 - `country` (str): An optional parameter representing the ISO Country Code. The default value is "US."
 
 - `filters` (str): An optional parameter that allows you to specify a list of keys to return in the app details. If not provided, it defaults to "basic." The available filter options include:
 
 - `basic` (Default): Returns essential information like type, name, steam_appid, required_age, is_free, dlc, detailed_description, short_description, about_the_game, supported_languages, header_image, website, pc_requirements, mac_requirements, and linux_requirements.
 
 - Optional filters (Specify one or more of these as a comma-separated string):
@@ -375,22 +376,21 @@
   - metacritic
   - categories
   - genres
   - screenshots
   - movies
   - recommendations
   - achievements
-Response
+    Response
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 terraria_app_id = 105600
 steam = Steam(KEY)
 
 # arguments: app_id
 user = steam.apps.get_app_details(terraria_app_id)
 
@@ -403,18 +403,15 @@
     "data": {
       "type": "game",
       "name": "Terraria",
       "steam_appid": 105600,
       "required_age": 0,
       "is_free": false,
       "controller_support": "full",
-      "dlc": [
-      409210,
-      1323320
-      ],
+      "dlc": [409210, 1323320],
       "detailed_description": "Dig, Fight, Explore, Build:  The very world is at your fingertips as you fight for survival, fortune, and glory.   Will you delve deep into cavernous expanses in search of treasure and raw materials with which to craft ever-evolving gear, machinery, and aesthetics?   Perhaps you will choose instead to seek out ever-greater foes to test your mettle in combat?   Maybe you will decide to construct your own city to house the host of mysterious allies you may encounter along your travels? <br><br>In the World of Terraria, the choice is yours!<br><br>Blending elements of classic action games with the freedom of sandbox-style creativity, Terraria is a unique gaming experience where both the journey and the destination are completely in the player’s control.   The Terraria adventure is truly as unique as the players themselves!  <br><br>Are you up for the monumental task of exploring, creating, and defending a world of your own?  <br><br>\t\t\t\t\t\t\t<strong>Key features:</strong><br>\t\t\t\t\t\t\t<ul class=\"bb_ul\"><li>Sandbox Play<br>\t\t\t\t\t\t\t</li><li> Randomly generated worlds<br>\t\t\t\t\t\t\t</li><li>Free Content Updates<br>\t\t\t\t\t\t\t</li></ul>",
       "about_the_game": "Dig, Fight, Explore, Build:  The very world is at your fingertips as you fight for survival, fortune, and glory.   Will you delve deep into cavernous expanses in search of treasure and raw materials with which to craft ever-evolving gear, machinery, and aesthetics?   Perhaps you will choose instead to seek out ever-greater foes to test your mettle in combat?   Maybe you will decide to construct your own city to house the host of mysterious allies you may encounter along your travels? <br><br>In the World of Terraria, the choice is yours!<br><br>Blending elements of classic action games with the freedom of sandbox-style creativity, Terraria is a unique gaming experience where both the journey and the destination are completely in the player’s control.   The Terraria adventure is truly as unique as the players themselves!  <br><br>Are you up for the monumental task of exploring, creating, and defending a world of your own?  <br><br>\t\t\t\t\t\t\t<strong>Key features:</strong><br>\t\t\t\t\t\t\t<ul class=\"bb_ul\"><li>Sandbox Play<br>\t\t\t\t\t\t\t</li><li> Randomly generated worlds<br>\t\t\t\t\t\t\t</li><li>Free Content Updates<br>\t\t\t\t\t\t\t</li></ul>",
       "short_description": "Dig, fight, explore, build! Nothing is impossible in this action-packed adventure game. Four Pack also available!",
       "supported_languages": "English, French, Italian, German, Spanish - Spain, Polish, Portuguese - Brazil, Russian, Simplified Chinese",
       "header_image": "https://cdn.akamai.steamstatic.com/steam/apps/105600/header.jpg?t=1666290860",
       "capsule_image": "https://cdn.akamai.steamstatic.com/steam/apps/105600/capsule_231x87.jpg?t=1666290860",
       "capsule_imagev5": "https://cdn.akamai.steamstatic.com/steam/apps/105600/capsule_184x69.jpg?t=1666290860",
@@ -435,67 +432,63 @@
   }
 }
 ```
 
 ### Getting user app stats
 
 ```python
-from steam import Steam
-from decouple import config
-
-KEY = config("STEAM_API_KEY")
+import os
+from steam_web_api import Steam
 
+KEY = os.environ.get("STEAM_API_KEY")
 
 steam = Steam(KEY)
 
 # arguments: steam_id, app_id
 user = steam.apps.get_user_stats("<steam_id>", "<app_id>")
 ```
 
 ### Getting user app achievements
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: steam_id, app_id
 user = steam.apps.get_user_achievements("<steam_id>", "<app_id>")
 ```
 
-
 ### Getting user ban status
 
 ```python
-from steam import Steam
-from decouple import config
+import os
+from steam_web_api import Steam
 
-KEY = config("STEAM_API_KEY")
+KEY = os.environ.get("STEAM_API_KEY")
 
 
 steam = Steam(KEY)
 
 # arguments: steam_id
 user = steam.users.get_player_bans("<steam_id>")
-````
-
+```
 
 ```json
 {
-"players":[
+  "players": [
     {
-    "SteamId":"76561198079362196",
-    "CommunityBanned":false,
-    "VACBanned":false,
-    "NumberOfVACBans":0,
-    "DaysSinceLastBan":0,
-    "NumberOfGameBans":0,
-    "EconomyBan":"none"
+      "SteamId": "76561198079362196",
+      "CommunityBanned": false,
+      "VACBanned": false,
+      "NumberOfVACBans": 0,
+      "DaysSinceLastBan": 0,
+      "NumberOfGameBans": 0,
+      "EconomyBan": "none"
     }
-    ]
+  ]
 }
 ```
-
```

### Comparing `python-steam-api-1.2.2/steam/apps.py` & `python-steam-api-2.0/steam_web_api/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import json
-
 import typing
-from requests import request, Response
-from .client import Client
-from .utils import buildUrlWithParamsForSearch
+
 from bs4 import BeautifulSoup
+from requests import Response, request
+
+from .client import Client
 from .constants import API_APP_DETAILS_URL, API_APP_SEARCH_URL
+from .utils import buildUrlWithParamsForSearch
 
 
 class Apps:
     """Steam Apps API client"""
 
     def __init__(self, client: Client):
         """Constructor for Steam Apps class"""
         self.__client = client
         self.__search_url = API_APP_SEARCH_URL
         self.__app_details_url = API_APP_DETAILS_URL
 
     def get_app_details(self, app_id: int, country="US", filters: typing.Optional[str] = "basic") -> dict:
         """Obtains an apps details
-        
+
         Args:
             app_id (int): App ID. For example 546560 (Half-Life-Alyx)
             country (str): ISO Country Code
             filters (str): list of keys to return, e.g. "name,platforms,price_overview". If you use multiple appids, you must set this parameter to "price_overview".
                 The filter basic returns the following keys:
                     type
                     name
@@ -59,29 +60,29 @@
         response = request("get", self.__app_details_url, params={"appids": app_id, "cc": country, "filters": filters})
         json_loaded_response = json.loads(response.text)
         return json_loaded_response
 
     def get_user_stats(self, steam_id: int, app_id: int) -> dict:
         """Obtains a user's stats for a specific app, includes only completed achievements
         along with app specific information
-        
+
         Args:
             steam_id (int): Steam 64 ID
             app_id (int): App ID
         """
         response = self.__client.request(
             "get",
             "/ISteamUserStats/GetUserStatsForGame/v2/",
             params={"steamid": steam_id, "appid": app_id},
         )
         return response
 
     def get_user_achievements(self, steam_id: int, app_id: int) -> dict:
         """Obtains information of the user's achievments in the app
-        
+
         Args:
             steam_id (int): Steam 64 ID
             app_id (int): App ID
         """
         response = self.__client.request(
             "get",
             "/ISteamUserStats/GetPlayerAchievements/v1/",
@@ -98,22 +99,22 @@
         """
         url = self.search_url(term, country)
         result = request("get", url)
         html = self.__validator(result)
         soup = BeautifulSoup(html, features="html.parser")
         links = soup.find_all("a")
         apps = []
-        for l in links:
-            if l.has_attr("data-ds-appid"):
+        for link in links:
+            if link.has_attr("data-ds-appid"):
                 app = {}
-                string_id = l["data-ds-appid"]
-                href = l["href"].replace("\\", "").replace('"', "")
-                app["id"] = [int(i) for i in string_id.replace("\\", "").replace('"', "").split(',')]
+                string_id = link["data-ds-appid"]
+                href = link["href"].replace("\\", "").replace('"', "")
+                app["id"] = [int(i) for i in string_id.replace("\\", "").replace('"', "").split(",")]
                 app["link"] = href
-                divs = l.select("div")
+                divs = link.select("div")
                 for div in divs:
                     if div["class"][0] == '\\"match_name\\"':
                         app["name"] = div.text
                     if div["class"][0] == '\\"match_price\\"':
                         app["price"] = div.text
                     if div["class"][0] == '\\"match_img\\"':
                         app["img"] = div.img["src"].replace("\\", "").replace('"', "")
@@ -129,15 +130,15 @@
 
     def __validator(self, result: Response) -> typing.Union[str, dict]:
         try:
             body = json.dumps(result.text)
         except Exception:
             body = {}
 
-        if type(body) is dict and body.get("code", None) is not None:
+        if isinstance(body, dict) and body.get("code", None) is not None:
             raise Exception(body.get("description"))
         elif result.status_code >= 400:
             raise Exception(" ".join([str(result.status_code), result.reason]))
         elif len(result.text) == 0:
             return "OK"
         else:
             return body
```

### Comparing `python-steam-api-1.2.2/steam/client.py` & `python-steam-api-2.0/steam_web_api/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,45 @@
 import json
+import typing
 
 import requests
-import typing
+
 from .constants import API_BASE_URL
 from .utils import buildUrlWithParams, mergeDict, retry
 
 
-class Client(object):
+class Client:
     """Steams API HTTP client"""
 
     def __init__(self, key: str, headers: dict = {}):
         """Constructor for TypeForm API client"""
         self.__headers = mergeDict(
             {
                 "Content-Type": "application/json",
                 "Accept": "application/json",
             },
             headers,
         )
         self.key = key
 
     @retry(times=3, exceptions=(ValueError, TypeError))
-    def request(
-        self, method: str, url: str, data: any = {}, params: dict = {}, headers={}
-    ) -> typing.Union[str, dict]:
-
+    def request(self, method: str, url: str, data: any = {}, params: dict = {}, headers={}) -> typing.Union[str, dict]:
         requestUrl = buildUrlWithParams((API_BASE_URL + url), self.key, params)
-
         requestHeaders = mergeDict(self.__headers, headers)
-        requestData = ""
-        if type(data) is dict:
-            requestData = json.dumps(data) if len(data.keys()) > 0 else ""
-
-        if type(data) is list:
-            requestData = json.dumps(data) if len(data) > 0 else ""
-
-        result = requests.request(
-            method, requestUrl, data=requestData, headers=requestHeaders
-        )
+        requestData = json.dumps(data) if len(data.keys()) > 0 else ""
+        result = requests.request(method, requestUrl, data=requestData, headers=requestHeaders)
         return self.__validator(result)
 
     def __validator(self, result: requests.Response) -> typing.Union[str, dict]:
         try:
             body = json.loads(result.text)
         except Exception:
             body = {}
 
-        if type(body) is dict and body.get("code", None) is not None:
+        if isinstance(body, dict) and body.get("code", None) is not None:
             raise Exception(body.get("description"))
         elif result.status_code >= 400:
             raise Exception(" ".join([str(result.status_code), result.reason]))
         elif len(result.text) == 0:
             return "OK"
         else:
             return body
```

### Comparing `python-steam-api-1.2.2/steam/users.py` & `python-steam-api-2.0/steam_web_api/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import json
-import typing
-from urllib import response
 from .client import Client
 
 
 class Users:
     """Steam Users API client"""
 
     def __init__(self, client: Client):
@@ -63,17 +60,15 @@
         response = self.__client.request(
             "get",
             "/IPlayerService/GetRecentlyPlayedGames/v1/",
             params={"steamid": steam_id},
         )["response"]
         return response
 
-    def get_owned_games(
-            self, steam_id: str, include_appinfo=True, includ_free_games=True
-    ) -> dict:
+    def get_owned_games(self, steam_id: str, include_appinfo=True, includ_free_games=True) -> dict:
         """Gets all owned games of a user by steam id
 
         Args:
             steam_id (str): Steam 64 ID
             include_appinfo (bool, optional): Includes app/game info. Defaults to True.
             includ_free_games (bool, optional): Includes free games. Defaults to True.
         """
@@ -155,24 +150,20 @@
         )
         return response
 
     def _transform_friends(self, friends_list: dict) -> dict:
         friend_steam_ids = [friend["steamid"] for friend in friends_list["friends"]]
         friends = self.get_user_details(",".join(friend_steam_ids), False)["players"]
         for f in friends:
-            found = next(
-                item
-                for item in friends_list["friends"]
-                if item["steamid"] == f["steamid"]
-            )
+            found = next(item for item in friends_list["friends"] if item["steamid"] == f["steamid"])
             f["relationship"] = found["relationship"]
             f["friend_since"] = found["friend_since"]
 
         return friends
-    
+
     def get_steamid(self, vanity: str) -> dict:
         """Get steamid64 from vanity URL
 
         Args:
             vanity (str): Vanity URL
         """
         response = self.__client.request(
```

### Comparing `python-steam-api-1.2.2/steam/utils.py` & `python-steam-api-2.0/steam_web_api/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 from urllib.parse import urlencode
 
 
 def buildUrlWithParams(url: str, key: str, params={}) -> str:
     encoded = urlencode(cleanDict(params))
-    return (
-        url + "?key=" + key
-        if (len(encoded) == 0)
-        else (url + "?key=" + key + "&" + encoded)
-    )
+    return url + "?key=" + key if (len(encoded) == 0) else (url + "?key=" + key + "&" + encoded)
 
 
 def buildUrlWithParamsForSearch(url: str, search: str, params={}) -> str:
     encoded = urlencode(cleanDict(params))
-    return (
-        url + "?term=" + search
-        if (len(encoded) == 0)
-        else (url + "?term=" + search + "&" + encoded)
-    )
+    return url + "?term=" + search if (len(encoded) == 0) else (url + "?term=" + search + "&" + encoded)
 
 
 def cleanDict(x: dict = {}) -> dict:
     result = {}
     for key in x:
         if x[key] is not None:
             # Check If List
@@ -50,22 +42,22 @@
     Retries the wrapped function/method `times` times if the exceptions listed
     in ``exceptions`` are thrown
     :param times: The number of times to repeat the wrapped function/method
     :type times: Int
     :param Exceptions: Lists of exceptions that trigger a retry attempt
     :type Exceptions: Tuple of Exceptions
     """
+
     def decorator(func):
         def newfn(*args, **kwargs):
             attempt = 0
             while attempt < times:
                 try:
                     return func(*args, **kwargs)
                 except exceptions:
-                    print(
-                        'Exception thrown when attempting to run %s, attempt '
-                        '%d of %d' % (func, attempt, times)
-                    )
+                    print("Exception thrown when attempting to run %s, attempt " "%d of %d" % (func, attempt, times))
                     attempt += 1
             return func(*args, **kwargs)
+
         return newfn
-    return decorator
+
+    return decorator
```

