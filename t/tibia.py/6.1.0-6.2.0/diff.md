# Comparing `tmp/tibia.py-6.1.0.tar.gz` & `tmp/tibia.py-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibia.py-6.1.0.tar", last modified: Tue Jan 16 02:01:12 2024, max compression
+gzip compressed data, was "tibia.py-6.2.0.tar", last modified: Sun Mar 31 22:03:06 2024, max compression
```

## Comparing `tibia.py-6.1.0.tar` & `tibia.py-6.2.0.tar`

### file list

```diff
@@ -1,93 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 02:01:12.689292 tibia.py-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    24454 2024-01-16 02:01:00.000000 tibia.py-6.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-01-16 02:01:00.000000 tibia.py-6.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-16 02:01:00.000000 tibia.py-6.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-01-16 02:01:12.689292 tibia.py-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-01-16 02:01:00.000000 tibia.py-6.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-01-16 02:01:00.000000 tibia.py-6.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-16 02:01:00.000000 tibia.py-6.1.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-16 02:01:00.000000 tibia.py-6.1.0/requirements-linting.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-16 02:01:00.000000 tibia.py-6.1.0/requirements-server.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-16 02:01:00.000000 tibia.py-6.1.0/requirements-testing.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-16 02:01:00.000000 tibia.py-6.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 02:01:12.689292 tibia.py-6.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 02:01:12.673292 tibia.py-6.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_bazaar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_character.py
--rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_creature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_forums.py
--rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_highscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_house.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_kill_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_leaderboards.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_spell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_tibiapy.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    14581 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tests/tests_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 02:01:12.685292 tibia.py-6.1.0/tibia.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-01-16 02:01:12.000000 tibia.py-6.1.0/tibia.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-01-16 02:01:12.000000 tibia.py-6.1.0/tibia.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 02:01:12.000000 tibia.py-6.1.0/tibia.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-16 02:01:12.000000 tibia.py-6.1.0/tibia.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-16 02:01:12.000000 tibia.py-6.1.0/tibia.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 02:01:12.677292 tibia.py-6.1.0/tibiapy/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 02:01:12.677292 tibia.py-6.1.0/tibiapy/builders/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/bazaar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/creature.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/highscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/house.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/kill_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/news.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/spell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/builders/world.py
--rw-r--r--   0 runner    (1001) docker     (127)    54985 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15592 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 02:01:12.681292 tibia.py-6.1.0/tibiapy/models/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/bazaar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/creature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/highscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/house.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/kill_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/spell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/tibia_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/models/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 02:01:12.685292 tibia.py-6.1.0/tibiapy/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29448 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/bazaar.py
--rw-r--r--   0 runner    (1001) docker     (127)    13817 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/character.py
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/creature.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    29196 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/highscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/house.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/kill_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/news.py
--rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/spell.py
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/parsers/world.py
--rw-r--r--   0 runner    (1001) docker     (127)    19231 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20426 2024-01-16 02:01:00.000000 tibia.py-6.1.0/tibiapy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.755630 tibia.py-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    24552 2024-03-31 22:02:58.000000 tibia.py-6.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-03-31 22:02:58.000000 tibia.py-6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-31 22:02:58.000000 tibia.py-6.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-03-31 22:03:06.755630 tibia.py-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-31 22:02:58.000000 tibia.py-6.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-03-31 22:02:58.000000 tibia.py-6.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-31 22:02:58.000000 tibia.py-6.2.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-31 22:02:58.000000 tibia.py-6.2.0/requirements-linting.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-31 22:02:58.000000 tibia.py-6.2.0/requirements-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-31 22:02:58.000000 tibia.py-6.2.0/requirements-testing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-31 22:02:58.000000 tibia.py-6.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 22:03:06.755630 tibia.py-6.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.743630 tibia.py-6.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_creature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_fansites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_forums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_highscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_house.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_leaderboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_tibiapy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14581 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.751630 tibia.py-6.2.0/tibia.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-03-31 22:03:06.000000 tibia.py-6.2.0/tibia.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-31 22:03:06.000000 tibia.py-6.2.0/tibia.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 22:03:06.000000 tibia.py-6.2.0/tibia.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-31 22:03:06.000000 tibia.py-6.2.0/tibia.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-31 22:03:06.000000 tibia.py-6.2.0/tibia.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.743630 tibia.py-6.2.0/tibiapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.747630 tibia.py-6.2.0/tibiapy/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14708 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/creature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/house.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/world.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56099 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15773 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.751630 tibia.py-6.2.0/tibiapy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/creature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/fansite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/house.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/tibia_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.751630 tibia.py-6.2.0/tibiapy/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29869 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13897 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/creature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/fansite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29449 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19036 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/house.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/world.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19460 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20410 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/utils.py
```

### Comparing `tibia.py-6.1.0/CHANGELOG.rst` & `tibia.py-6.2.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 Changelog
 =========
 
 .. note::
     Due to this library relying on external content, older versions are not guaranteed to work.
     Try to always use the latest version.
 
+.. v6.2.0
+
+6.2.0 (2024-03-31)
+==================
+- Add support for parsing the fansites section.
+
 .. v6.1.0
 
 6.1.0 (2024-01-15)
 ==================
 - Add revealed gems to auction details.
 - Fixed `get_highscores` not handling null values in parameters.
 - Fixed house parsing not handing guildhalls properly.
```

### Comparing `tibia.py-6.1.0/LICENSE` & `tibia.py-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/README.md` & `tibia.py-6.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # Tibia.py
 An API to parse Tibia.com content into object oriented data.
 
 No fetching is done by this module, you must provide the html content.
 
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Galarzaa90/tibia.py/build.yml)
-[![codecov](https://codecov.io/gh/Galarzaa90/tibia.py/branch/master/graph/badge.svg?token=mS9Wxv6O2F)](https://codecov.io/gh/Galarzaa90/tibia.py)
 [![PyPI](https://img.shields.io/pypi/v/tibia.py.svg)](https://pypi.python.org/pypi/tibia.py/)
+![GitHub commits since latest release (branch)](https://img.shields.io/github/commits-since/Galarzaa90/tibia.py/latest/main)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tibia.py.svg)
 ![PyPI - License](https://img.shields.io/pypi/l/tibia.py.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/tibia.py)
 
+[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=Galarzaa90_tibia.py&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=Galarzaa90_tibia.py)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=Galarzaa90_tibia.py&metric=coverage)](https://sonarcloud.io/summary/new_code?id=Galarzaa90_tibia.py)
+[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=Galarzaa90_tibia.py&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=Galarzaa90_tibia.py)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=Galarzaa90_tibia.py&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=Galarzaa90_tibia.py)
+[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=Galarzaa90_tibia.py&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=Galarzaa90_tibia.py)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=Galarzaa90_tibia.py&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=Galarzaa90_tibia.py)
 
 **Features:**
 
 - Converts data into well-structured Python objects.
 - Type consistent attributes.
 - All objects can be converted to JSON strings.
 - Can be used with any networking library.
```

### Comparing `tibia.py-6.1.0/pyproject.toml` & `tibia.py-6.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     'Natural Language :: English',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Programming Language :: Python',
     'Topic :: Games/Entertainment :: Role-Playing',
     'Topic :: Internet',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development',
@@ -87,65 +88,14 @@
     "return NotImplemented",
     "if TYPE_CHECKING:",
     "logger.debug\\(.*",
     "\\.{3}",
 ]
 
 
-[tool.flake8]
-max-line-length = 120
-exclude = [
-    "__pycache__",
-    ".git/",
-    "build/",
-    ".idea/",
-    "venv/",
-    "docs/",
-    "logs/",
-    "tests/",
-]
-tee = true
-# Ignore unused imports in __INIT__.py files
-per-file-ignores = [
-    "**/__init__.py:F401, F403",
-    "server.py:D103,B008,TC002",
-    "**/builders/*:D101",
-]
-count = true
-ignore = [
-    # flake8-docstrings: Missing docstring in public module
-    "D100",
-    # flake8-docstrings: Missing docstring in public method
-    "D102",
-    # flake8-docstrings: Missing docstring in public package
-    "D104",
-    # flake8-docstrings: Missing docstring in magic method
-    "D105",
-    # flake8-docstrings: Missing docstring in __init__
-    "D107",
-    # flake8: line break before binary operator
-    "W503",
-    # flake8: line too long (121 > 120 characters)
-    "E501",
-]
-rst-roles = [
-    "class",
-    "py:attr",
-    "obj",
-    "meth",
-    "attr",
-    "exc",
-]
-rst-directives = [
-    "versionadded",
-    "versionchanged",
-]
-literal-inline-quotes = "double"
-type-checking-pydantic-enabled = true
-
 [tool.ruff]
 exclude = [
     "__pycache__",
     ".git/",
     "build/",
     ".idea/",
     "venv/",
@@ -217,22 +167,25 @@
     "D203",
     # 1 blank line required before class docstring
     "D213",
     # Mutable class attributes should be annotated with `typing.ClassVar`
     "RUF012",
     # PEP 484 prohibits implicit `Optional`
     "RUF013",
+
     # Missing type annotation for {name} in method
     "ANN101",
     # Missing type annotation for {name} in classmethod
     "ANN102",
     # Missing return type annotation for private function {name}
     "ANN202",
     # Missing return type annotation for special method {name}
     "ANN204",
+    # Dynamically typed expressions ({name}) are disallowed in `other`
+    "ANN401",
 ]
 
 
 [tool.ruff.lint.pycodestyle]
 max-line-length = 120
 
 [tool.ruff.lint.pep8-naming]
```

### Comparing `tibia.py-6.1.0/tests/tests_bazaar.py` & `tibia.py-6.2.0/tests/tests_bazaar.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_character.py` & `tibia.py-6.2.0/tests/tests_character.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_client.py` & `tibia.py-6.2.0/tests/tests_client.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_creature.py` & `tibia.py-6.2.0/tests/tests_creature.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_enums.py` & `tibia.py-6.2.0/tests/tests_enums.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_events.py` & `tibia.py-6.2.0/tests/tests_events.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_forums.py` & `tibia.py-6.2.0/tests/tests_forums.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_guild.py` & `tibia.py-6.2.0/tests/tests_guild.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_highscores.py` & `tibia.py-6.2.0/tests/tests_highscores.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_house.py` & `tibia.py-6.2.0/tests/tests_house.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_kill_statistics.py` & `tibia.py-6.2.0/tests/tests_kill_statistics.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_leaderboards.py` & `tibia.py-6.2.0/tests/tests_leaderboards.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_news.py` & `tibia.py-6.2.0/tests/tests_news.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_spell.py` & `tibia.py-6.2.0/tests/tests_spell.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_tibiapy.py` & `tibia.py-6.2.0/tests/tests_tibiapy.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_utils.py` & `tibia.py-6.2.0/tests/tests_utils.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tests/tests_world.py` & `tibia.py-6.2.0/tests/tests_world.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibia.py.egg-info/SOURCES.txt` & `tibia.py-6.2.0/tibia.py.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 requirements.txt
 tests/tests_bazaar.py
 tests/tests_character.py
 tests/tests_client.py
 tests/tests_creature.py
 tests/tests_enums.py
 tests/tests_events.py
+tests/tests_fansites.py
 tests/tests_forums.py
 tests/tests_guild.py
 tests/tests_highscores.py
 tests/tests_house.py
 tests/tests_kill_statistics.py
 tests/tests_leaderboards.py
 tests/tests_news.py
@@ -53,14 +54,15 @@
 tibiapy/builders/world.py
 tibiapy/models/__init__.py
 tibiapy/models/base.py
 tibiapy/models/bazaar.py
 tibiapy/models/character.py
 tibiapy/models/creature.py
 tibiapy/models/event.py
+tibiapy/models/fansite.py
 tibiapy/models/forum.py
 tibiapy/models/guild.py
 tibiapy/models/highscores.py
 tibiapy/models/house.py
 tibiapy/models/kill_statistics.py
 tibiapy/models/leaderboard.py
 tibiapy/models/news.py
@@ -69,14 +71,15 @@
 tibiapy/models/tibia_response.py
 tibiapy/models/world.py
 tibiapy/parsers/__init__.py
 tibiapy/parsers/bazaar.py
 tibiapy/parsers/character.py
 tibiapy/parsers/creature.py
 tibiapy/parsers/event.py
+tibiapy/parsers/fansite.py
 tibiapy/parsers/forum.py
 tibiapy/parsers/guild.py
 tibiapy/parsers/highscores.py
 tibiapy/parsers/house.py
 tibiapy/parsers/kill_statistics.py
 tibiapy/parsers/leaderboard.py
 tibiapy/parsers/news.py
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/bazaar.py` & `tibia.py-6.2.0/tibiapy/builders/bazaar.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         self._type = type
         return self
 
     def filters(self, filters: AuctionFilters) -> Self:
         self._filters = filters
         return self
 
-    def build(self):
+    def build(self) -> CharacterBazaar:
         return CharacterBazaar(
             current_page=self._current_page,
             total_pages=self._total_pages,
             results_count=self._results_count,
             entries=self._entries,
             type=self._type,
             filters=self._filters,
@@ -139,15 +139,15 @@
         self._bid_type = bid_type
         return self
 
     def status(self, status: AuctionStatus) -> Self:
         self._status = status
         return self
 
-    def build(self):
+    def build(self) -> Auction:
         return Auction(
             auction_id=self._auction_id,
             name=self._name,
             level=self._level,
             world=self._world,
             vocation=self._vocation,
             sex=self._sex,
@@ -395,15 +395,15 @@
         self._bosstiary_progress = bosstiary_progress
         return self
 
     def add_revealed_gem(self, gem: RevealedGem) -> Self:
         self._revealed_gems.append(gem)
         return self
 
-    def build(self):
+    def build(self) -> AuctionDetails:
         return AuctionDetails(
             hit_points=self._hit_points,
             mana=self._mana,
             capacity=self._capacity,
             speed=self._speed,
             blessings_count=self._blessings_count,
             mounts_count=self._mounts_count,
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/character.py` & `tibia.py-6.2.0/tibiapy/builders/character.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         self._other_characters.append(other_character)
         return self
 
     def other_characters(self, other_characters: List[OtherCharacter]) -> Self:
         self._other_characters = other_characters
         return self
 
-    def build(self):
+    def build(self) -> Character:
         return Character(
             name=self._name,
             is_traded=self._traded,
             deletion_date=self._deletion_date,
             former_names=self._former_names,
             title=self._title,
             unlocked_titles=self._unlocked_titles,
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/creature.py` & `tibia.py-6.2.0/tibiapy/builders/creature.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self._name = name
         return self
 
     def identifier(self, identifier: str) -> Self:
         self._identifier = identifier
         return self
 
-    def build(self):
+    def build(self) -> CreatureEntry:
         return CreatureEntry(
             name=self._name,
             identifier=self._identifier,
         )
 
 
 class CreatureBuilder:
@@ -87,15 +87,15 @@
         self._summonable = summonable
         return self
 
     def convinceable(self, convinceable: bool) -> Self:
         self._convinceable = convinceable
         return self
 
-    def build(self):
+    def build(self) -> Creature:
         return Creature(
             name=self._name,
             identifier=self._identifier,
             description=self._description,
             hitpoints=self._hitpoints,
             experience=self._experience,
             immune_to=self._immune_to,
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/event.py` & `tibia.py-6.2.0/tibiapy/builders/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,13 +28,13 @@
         self._events = events
         return self
 
     def add_event(self, event: EventEntry) -> Self:
         self._events.append(event)
         return self
 
-    def build(self):
+    def build(self) -> EventSchedule:
         return EventSchedule(
             month=self._month,
             year=self._year,
             events=self._events,
         )
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/forum.py` & `tibia.py-6.2.0/tibiapy/builders/forum.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self._entries = entries
         return self
 
     def add_entry(self, entry) -> Self:
         self._entries.append(entry)
         return self
 
-    def build(self):
+    def build(self) -> CMPostArchive:
         return CMPostArchive(
             from_date=self._from_date,
             to_date=self._to_date,
             current_page=self._current_page,
             total_pages=self._total_pages,
             results_count=self._results_count,
             entries=self._entries,
@@ -75,15 +75,15 @@
         self._board = board
         return self
 
     def thread_title(self, thread_title) -> Self:
         self._thread_title = thread_title
         return self
 
-    def build(self):
+    def build(self) -> CMPost:
         return CMPost(
             post_id=self._post_id,
             posted_on=self._posted_on,
             board=self._board,
             thread_title=self._thread_title,
         )
 
@@ -137,15 +137,15 @@
         self._from_date = from_date
         return self
 
     def to_date(self, to_date) -> Self:
         self._to_date = to_date
         return self
 
-    def build(self):
+    def build(self) -> ForumAnnouncement:
         return ForumAnnouncement(
             announcement_id=self._announcement_id,
             board=self._board,
             section=self._section,
             board_id=self._board_id,
             section_id=self._section_id,
             author=self._author,
@@ -213,15 +213,15 @@
         self._entries = entries
         return self
 
     def add_entry(self, entry) -> Self:
         self._entries.append(entry)
         return self
 
-    def build(self):
+    def build(self) -> ForumBoard:
         return ForumBoard(
             board_id=self._board_id,
             name=self._name,
             section=self._section,
             section_id=self._section_id,
             current_page=self._current_page,
             total_pages=self._total_pages,
@@ -299,15 +299,15 @@
         self._anchored_post = anchored_post
         return self
 
     def add_entry(self, entry) -> Self:
         self._entries.append(entry)
         return self
 
-    def build(self):
+    def build(self) -> ForumThread:
         return ForumThread(
             title=self._title,
             thread_id=self._thread_id,
             board=self._board,
             board_id=self._board_id,
             section=self._section,
             section_id=self._section_id,
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/guild.py` & `tibia.py-6.2.0/tibiapy/builders/guild.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self._world = world
         return self
 
     def active(self, active: bool) -> Self:
         self._active = active
         return self
 
-    def build(self):
+    def build(self) -> GuildEntry:
         return GuildEntry(
             name=self._name,
             logo_url=self._logo_url,
             description=self._description,
             world=self._world,
             active=self._active,
         )
@@ -124,15 +124,15 @@
         self._invites = invites
         return self
 
     def add_invite(self, invite: GuildInvite) -> Self:
         self._invites.append(invite)
         return self
 
-    def build(self):
+    def build(self) -> Guild:
         return Guild(
             name=self._name,
             logo_url=self._logo_url,
             description=self._description,
             world=self._world,
             founded=self._founded,
             active=self._active,
@@ -162,15 +162,15 @@
         self._current = current
         return self
 
     def history(self, history: List[GuildWarEntry]) -> Self:
         self._history = history
         return self
 
-    def build(self):
+    def build(self) -> GuildWars:
         return GuildWars(
             name=self._name,
             history=self._history,
             is_current=self._current,
         )
 
 
@@ -233,15 +233,15 @@
         self._winner = winner
         return self
 
     def surrender(self, surrender: bool) -> Self:
         self._surrender = surrender
         return self
 
-    def build(self):
+    def build(self) -> GuildWarEntry:
         return GuildWarEntry(
             guild_name=self._guild_name,
             guild_score=self._guild_score,
             guild_fee=self._guild_fee,
             opponent_name=self._opponent_name,
             opponent_score=self._opponent_score,
             opponent_fee=self._opponent_fee,
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/highscores.py` & `tibia.py-6.2.0/tibiapy/builders/highscores.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self._entries.append(entry)
         return self
 
     def available_worlds(self, available_worlds: List[str]) -> Self:
         self._available_worlds = available_worlds
         return self
 
-    def build(self):
+    def build(self) -> Highscores:
         return Highscores(
             world=self._world,
             category=self._category,
             vocation=self._vocation,
             battleye_filter=self._battleye_filter,
             pvp_types_filter=self._pvp_types_filter,
             current_page=self._current_page,
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/house.py` & `tibia.py-6.2.0/tibiapy/builders/house.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 
 from typing import List, TYPE_CHECKING, Optional
 
+from typing_extensions import Self
+
 from tibiapy.models.house import HouseEntry, HousesSection, House
 
 if TYPE_CHECKING:
     import datetime
     from tibiapy.enums import HouseStatus, HouseType, HouseOrder, Sex
 
 
@@ -17,51 +19,51 @@
         self._status = None
         self._house_type = None
         self._order = None
         self._entries = []
         self._available_worlds = []
         self._available_towns = []
 
-    def world(self, world: str):
+    def world(self, world: str) -> Self:
         self._world = world
         return self
 
-    def town(self, town: str):
+    def town(self, town: str) -> Self:
         self._town = town
         return self
 
-    def status(self, status: HouseStatus):
+    def status(self, status: HouseStatus) -> Self:
         self._status = status
         return self
 
-    def house_type(self, house_type: HouseType):
+    def house_type(self, house_type: HouseType) -> Self:
         self._house_type = house_type
         return self
 
-    def order(self, order: HouseOrder):
+    def order(self, order: HouseOrder) -> Self:
         self._order = order
         return self
 
-    def entries(self, entries: List[HouseEntry]):
+    def entries(self, entries: List[HouseEntry]) -> Self:
         self._entries = entries
         return self
 
-    def add_entry(self, entry: HouseEntry):
+    def add_entry(self, entry: HouseEntry) -> Self:
         self._entries.append(entry)
         return self
 
-    def available_worlds(self, available_worlds: List[str]):
+    def available_worlds(self, available_worlds: List[str]) -> Self:
         self._available_worlds = available_worlds
         return self
 
-    def available_towns(self, available_towns: List[str]):
+    def available_towns(self, available_towns: List[str]) -> Self:
         self._available_towns = available_towns
         return self
 
-    def build(self):
+    def build(self) -> HousesSection:
         return HousesSection(
             world=self._world,
             town=self._town,
             status=self._status,
             house_type=self._house_type,
             order=self._order,
             entries=self._entries,
@@ -96,43 +98,43 @@
         self._size = None
         self._status = None
         self._type = None
         self._rent = None
         self._time_left = None
         self._highest_bid = None
 
-    def status(self, status: HouseStatus):
+    def status(self, status: HouseStatus) -> Self:
         self._status = status
         return self
 
-    def type(self, type: HouseType):
+    def type(self, type: HouseType) -> Self:
         self._type = type
         return self
 
-    def town(self, town: str):
+    def town(self, town: str) -> Self:
         self._town = town
         return self
 
-    def size(self, size: int):
+    def size(self, size: int) -> Self:
         self._size = size
         return self
 
-    def rent(self, rent: int):
+    def rent(self, rent: int) -> Self:
         self._rent = rent
         return self
 
-    def time_left(self, time_left: Optional[datetime.timedelta]):
+    def time_left(self, time_left: Optional[datetime.timedelta]) -> Self:
         self._time_left = time_left
         return self
 
-    def highest_bid(self, highest_bid: Optional[int]):
+    def highest_bid(self, highest_bid: Optional[int]) -> Self:
         self._highest_bid = highest_bid
         return self
 
-    def build(self):
+    def build(self) -> HouseEntry:
         return HouseEntry(
             name=self._name,
             id=self._id,
             world=self._world,
             status=self._status,
             type=self._type,
             town=self._town,
@@ -159,79 +161,79 @@
         self._transfer_recipient = None
         self._transfer_price = None
         self._transfer_accepted = None
         self._highest_bid = None
         self._highest_bidder = None
         self._auction_end = None
 
-    def status(self, status: HouseStatus):
+    def status(self, status: HouseStatus) -> Self:
         self._status = status
         return self
 
-    def rent(self, rent: int):
+    def rent(self, rent: int) -> Self:
         self._rent = rent
         return self
 
-    def type(self, type: HouseType):
+    def type(self, type: HouseType) -> Self:
         self._type = type
         return self
 
-    def image_url(self, image_url: str):
+    def image_url(self, image_url: str) -> Self:
         self._image_url = image_url
         return self
 
-    def beds(self, beds: int):
+    def beds(self, beds: int) -> Self:
         self._beds = beds
         return self
 
-    def size(self, size: int):
+    def size(self, size: int) -> Self:
         self._size = size
         return self
 
-    def owner(self, owner: Optional[str]):
+    def owner(self, owner: Optional[str]) -> Self:
         self._owner = owner
         return self
 
-    def owner_sex(self, owner_sex: Sex):
+    def owner_sex(self, owner_sex: Sex) -> Self:
         self._owner_sex = owner_sex
         return self
 
-    def paid_until(self, paid_until: Optional[datetime.datetime]):
+    def paid_until(self, paid_until: Optional[datetime.datetime]) -> Self:
         self._paid_until = paid_until
         return self
 
-    def transfer_date(self, transfer_date: Optional[datetime.datetime]):
+    def transfer_date(self, transfer_date: Optional[datetime.datetime]) -> Self:
         self._transfer_date = transfer_date
         return self
 
-    def transfer_recipient(self, transfer_recipient: Optional[str]):
+    def transfer_recipient(self, transfer_recipient: Optional[str]) -> Self:
         self._transfer_recipient = transfer_recipient
         return self
 
-    def transfer_price(self, transfer_price: Optional[int]):
+    def transfer_price(self, transfer_price: Optional[int]) -> Self:
         self._transfer_price = transfer_price
         return self
 
-    def transfer_accepted(self, transfer_accepted: Optional[bool]):
+    def transfer_accepted(self, transfer_accepted: Optional[bool]) -> Self:
         self._transfer_accepted = transfer_accepted
         return self
 
-    def highest_bid(self, highest_bid: Optional[int]):
+    def highest_bid(self, highest_bid: Optional[int]) -> Self:
         self._highest_bid = highest_bid
         return self
 
-    def highest_bidder(self, highest_bidder: Optional[str]):
+    def highest_bidder(self, highest_bidder: Optional[str]) -> Self:
         self._highest_bidder = highest_bidder
         return self
 
-    def auction_end(self, auction_end: Optional[datetime.datetime]):
+    def auction_end(self, auction_end: Optional[datetime.datetime]) -> Self:
         self._auction_end = auction_end
         return self
 
-    def build(self):
+    def build(self) -> House:
         return House(
             name=self._name,
             id=self._id,
             world=self._world,
             status=self._status,
             type=self._type,
             size=self._size,
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/kill_statistics.py` & `tibia.py-6.2.0/tibiapy/builders/kill_statistics.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         self._total = total
         return self
 
     def available_worlds(self, available_worlds: List[str]) -> Self:
         self._available_worlds = available_worlds
         return self
 
-    def build(self):
+    def build(self) -> KillStatistics:
         return KillStatistics(
             world=self._world,
             entries=self._entries,
             total=self._total,
             available_worlds=self._available_worlds,
         )
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/leaderboard.py` & `tibia.py-6.2.0/tibiapy/builders/leaderboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self._total_pages = total_pages
         return self
 
     def results_count(self, results_count: int) -> Self:
         self._results_count = results_count
         return self
 
-    def build(self):
+    def build(self) -> Leaderboard:
         return Leaderboard(
             world=self._world,
             available_worlds=self._available_worlds,
             rotation=self._rotation,
             available_rotations=self._available_rotations,
             entries=self._entries,
             last_updated=self._last_updated,
@@ -91,13 +91,13 @@
         self._rank = rank
         return self
 
     def drome_level(self, drome_level: int) -> Self:
         self._drome_level = drome_level
         return self
 
-    def build(self):
+    def build(self) -> LeaderboardEntry:
         return LeaderboardEntry(
             name=self._name,
             rank=self._rank,
             drome_level=self._drome_level,
         )
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/news.py` & `tibia.py-6.2.0/tibiapy/builders/news.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self._entries = entries
         return self
 
     def add_entry(self, entry: NewsEntry) -> Self:
         self._entries.append(entry)
         return self
 
-    def build(self):
+    def build(self) -> NewsArchive:
         return NewsArchive(
             from_date=self._from_date,
             to_date=self._to_date,
             types=self._types,
             categories=self._categories,
             entries=self._entries,
         )
@@ -89,15 +89,15 @@
         self._content = content
         return self
 
     def thread_id(self, thread_id: Optional[int]) -> Self:
         self._thread_id = thread_id
         return self
 
-    def build(self):
+    def build(self) -> News:
         return News(
             id=self._id,
             category=self._category,
             title=self._title,
             published_on=self._published_on,
             content=self._content,
             thread_id=self._thread_id,
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/spell.py` & `tibia.py-6.2.0/tibiapy/builders/spell.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self._entries = entries
         return self
 
     def add_entry(self, spell: SpellEntry) -> Self:
         self._entries.append(spell)
         return self
 
-    def build(self):
+    def build(self) -> SpellsSection:
         return SpellsSection(
             vocation=self._vocation,
             group=self._group,
             spell_type=self._spell_type,
             is_premium=self._premium,
             sort_by=self._sort_by,
             entries=self._entries,
@@ -65,51 +65,51 @@
         self._group = None
         self._spell_type = None
         self._exp_level = None
         self._mana = None
         self._price = None
         self._is_premium = None
 
-    def identifier(self, identifier: str):
+    def identifier(self, identifier: str) -> Self:
         self._identifier = identifier
         return self
 
-    def name(self, name: str):
+    def name(self, name: str) -> Self:
         self._name = name
         return self
 
-    def words(self, words: str):
+    def words(self, words: str) -> Self:
         self._words = words
         return self
 
-    def group(self, group: SpellGroup):
+    def group(self, group: SpellGroup) -> Self:
         self._group = group
         return self
 
-    def spell_type(self, spell_type: SpellType):
+    def spell_type(self, spell_type: SpellType) -> Self:
         self._spell_type = spell_type
         return self
 
-    def exp_level(self, exp_level: int):
+    def exp_level(self, exp_level: int) -> Self:
         self._exp_level = exp_level
         return self
 
-    def mana(self, mana: Optional[int]):
+    def mana(self, mana: Optional[int]) -> Self:
         self._mana = mana
         return self
 
-    def price(self, price: int):
+    def price(self, price: int) -> Self:
         self._price = price
         return self
 
-    def is_premium(self, is_premium: bool):
+    def is_premium(self, is_premium: bool) -> Self:
         self._is_premium = is_premium
         return self
 
-    def build(self):
+    def build(self) -> SpellEntry:
         return SpellEntry(
             identifier=self._identifier,
             name=self._name,
             words=self._words,
             group=self._group,
             spell_type=self._spell_type,
             exp_level=self._exp_level,
@@ -175,15 +175,15 @@
         self._cities = cities
         return self
 
     def rune(self, rune: Rune) -> Self:
         self._rune = rune
         return self
 
-    def build(self):
+    def build(self) -> Spell:
         return Spell(
             identifier=self._identifier,
             name=self._name,
             words=self._words,
             group=self._group,
             spell_type=self._spell_type,
             exp_level=self._exp_level,
@@ -238,15 +238,15 @@
         self._magic_level = magic_level
         return self
 
     def magic_type(self, magic_type: Optional[str]) -> Self:
         self._magic_type = magic_type
         return self
 
-    def build(self):
+    def build(self) -> Rune:
         return Rune(
             name=self._name,
             vocations=self._vocations,
             group=self._group,
             exp_level=self._exp_level,
             mana=self._mana,
             magic_level=self._magic_level,
```

### Comparing `tibia.py-6.1.0/tibiapy/builders/world.py` & `tibia.py-6.2.0/tibiapy/builders/world.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self._battleye_type = battleye_type
         return self
 
     def is_experimental(self, is_experimental: bool) -> Self:
         self._is_experimental = is_experimental
         return self
 
-    def build(self):
+    def build(self) -> WorldEntry:
         return WorldEntry(
             name=self._name,
             is_online=self._is_online,
             online_count=self._online_count,
             location=self._location,
             pvp_type=self._pvp_type,
             is_premium_only=self._is_premium_only,
@@ -119,15 +119,15 @@
         self._online_players = online_players
         return self
 
     def add_online_player(self, player: OnlineCharacter) -> Self:
         self._online_players.append(player)
         return self
 
-    def build(self):
+    def build(self) -> World:
         return World(
             name=self._name,
             is_online=self._is_online,
             online_count=self._online_count,
             record_count=self._record_count,
             record_date=self._record_date,
             creation_date=self._creation_date,
@@ -157,13 +157,13 @@
         self._record_date = record_date
         return self
 
     def worlds(self, worlds: List[WorldEntry]) -> Self:
         self._worlds = worlds
         return self
 
-    def build(self):
+    def build(self) -> WorldOverview:
         return WorldOverview(
             record_count=self._record_count,
             record_date=self._record_date,
             worlds=self._worlds,
         )
```

### Comparing `tibia.py-6.1.0/tibiapy/client.py` & `tibia.py-6.2.0/tibiapy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,48 +2,50 @@
 from __future__ import annotations
 
 import asyncio
 import datetime
 import json
 import logging
 import time
-from typing import Callable, Optional, Set, TYPE_CHECKING, TypeVar
+from typing import Any, Callable, Dict, Optional, Set, TYPE_CHECKING, TypeVar
 
 import aiohttp
 import aiohttp_socks
 
 import tibiapy
 from tibiapy.enums import (BazaarType, HighscoresBattlEyeType, HighscoresCategory, HighscoresProfession, HouseOrder,
                            HouseStatus, HouseType, NewsCategory, NewsType, PvpTypeFilter, SpellGroup, SpellSorting,
                            SpellType, SpellVocationFilter)
 from tibiapy.errors import ForbiddenError, NetworkError, SiteMaintenanceError
 from tibiapy.models import TibiaResponse
 from tibiapy.parsers import (
     AuctionParser, BoostableBossesParser, BoostedCreaturesParser, CMPostArchiveParser, CharacterBazaarParser,
-    CharacterParser, CreatureParser, CreaturesSectionParser, EventScheduleParser, ForumAnnouncementParser,
+    CharacterParser, CreatureParser, CreaturesSectionParser, EventScheduleParser, FansitesSectionParser,
+    ForumAnnouncementParser,
     ForumBoardParser, ForumSectionParser, ForumThreadParser, GuildParser, GuildWarsParser, GuildsSectionParser,
     HighscoresParser, HouseParser, HousesSectionParser, KillStatisticsParser, LeaderboardParser, NewsArchiveParser,
     NewsParser, SpellParser, SpellsSectionParser, WorldOverviewParser, WorldParser,
 )
 from tibiapy.urls import (
     get_auction_url, get_bazaar_url, get_boostable_bosses_url, get_character_url, get_cm_post_archive_url,
     get_community_boards_url, get_creature_url, get_creatures_section_url, get_event_schedule_url,
-    get_forum_announcement_url, get_forum_board_url, get_forum_post_url, get_forum_section_url, get_forum_thread_url,
+    get_fansites_url, get_forum_announcement_url, get_forum_board_url, get_forum_post_url, get_forum_section_url,
+    get_forum_thread_url,
     get_guild_url, get_guild_wars_url, get_highscores_url, get_house_url, get_houses_section_url,
     get_kill_statistics_url, get_leaderboards_url, get_news_archive_url, get_news_url, get_spell_url,
     get_spells_section_url, get_support_boards_url, get_trade_boards_url, get_world_boards_url, get_world_guilds_url,
     get_world_overview_url, get_world_url,
 )
 
 if TYPE_CHECKING:
     from tibiapy.models import (
         AjaxPaginator, Auction, AuctionFilters, BoostableBosses, BoostedCreatures, BossEntry, CMPostArchive, Character,
-        CharacterBazaar, Creature, CreatureEntry, CreaturesSection, EventSchedule, ForumAnnouncement, ForumBoard,
-        ForumSection, ForumThread, Guild, GuildWars, GuildsSection, Highscores, House, HousesSection, KillStatistics,
-        Leaderboard, News, NewsArchive, Spell, SpellsSection, World, WorldOverview,
+        CharacterBazaar, Creature, CreatureEntry, CreaturesSection, EventSchedule, FansitesSection, ForumAnnouncement,
+        ForumBoard, ForumSection, ForumThread, Guild, GuildWars, GuildsSection, Highscores, House, HousesSection,
+        KillStatistics, Leaderboard, News, NewsArchive, Spell, SpellsSection, World, WorldOverview,
     )
 
 __all__ = (
     "Client",
 )
 
 T = TypeVar("T")
@@ -126,25 +128,33 @@
             loop=self.loop,
             headers=headers,
             connector=connector,
         )
         self._session_ready.set()
 
     @classmethod
-    def _handle_status(cls, status_code: int, fetching_time: float = 0.0):
+    def _handle_status(cls, status_code: int, fetching_time: float = 0.0) -> None:
         """Handle error status codes, raising exceptions if necessary."""
         if status_code < 400:
             return
 
         if status_code == 403:
             raise ForbiddenError("403 Forbidden: Might be getting rate-limited", fetching_time=fetching_time)
 
         raise NetworkError(f"Request error, status code: {status_code:d}", fetching_time=fetching_time)
 
-    async def _request(self, method, url, data=None, headers=None, *, test: bool = False):
+    async def _request(
+            self,
+            method: str,
+            url: str,
+            data: Dict[str, Any] = None,
+            headers: Dict[str, Any] = None,
+            *,
+            test: bool = False,
+    ):
         """Perform the HTTP request, handling possible error statuses.
 
         Parameters
         ----------
         method: :class:`str`
             The HTTP method to use for the request.
         url: :class:`str`
@@ -189,15 +199,15 @@
         except aiohttp.ClientError as e:
             raise NetworkError(f"aiohttp.ClientError: {e}", e, time.perf_counter() - init_time) from e
         except aiohttp_socks.SocksConnectionError as e:
             raise NetworkError(f"aiohttp_socks.SocksConnectionError: {e}", e, time.perf_counter() - init_time) from e
         except UnicodeDecodeError as e:
             raise NetworkError(f"UnicodeDecodeError: {e}", e, time.perf_counter() - init_time) from e
 
-    async def _fetch_all_pages(self, auction_id: int, paginator: AjaxPaginator, item_type, *, test: bool = False):
+    async def _fetch_all_pages(self, auction_id: int, paginator: AjaxPaginator, item_type: int, *, test: bool = False):
         """Fetch all the pages of an auction paginator.
 
         Parameters
         ----------
         auction_id: :class:`int`
             The id of the auction.
         paginator:
@@ -215,15 +225,15 @@
                 entries = AuctionParser._parse_page_items(content, paginator)
                 paginator.entries.extend(entries)
 
             current_page += 1
 
         paginator.is_fully_fetched = True
 
-    async def _fetch_ajax_page(self, auction_id, type_id, page, *, test: bool = False):
+    async def _fetch_ajax_page(self, auction_id: int, type_id: int, page: int, *, test: bool = False):
         """Fetch an ajax page from the paginated summaries in the auction section.
 
         Parameters
         ----------
         auction_id: :class:`int`
             The id of the auction.
         type_id: :class:`int`
@@ -1031,14 +1041,40 @@
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
         response = await self._request("GET", get_guild_wars_url(name), test=test)
         return response.parse(GuildWarsParser.from_content)
 
+    async def fetch_fansites_section(self, *, test: bool = False) -> TibiaResponse[FansitesSection]:
+        """Fetch the fansites section from Tibia.com.
+
+        .. versionadded:: 6.2.0
+
+        Parameters
+        ----------
+        test:
+            Whether to request the test website instead.
+
+        Returns
+        -------
+        TibiaResponse[FansitesSection]
+            A response containing the fansites section.
+
+        Raises
+        ------
+        Forbidden
+            If a 403 Forbidden error was returned.
+            This usually means that Tibia.com is rate-limiting the client because of too many requests.
+        NetworkError
+            If there's any connection errors during the request.
+        """
+        response = await self._request("GET", get_fansites_url(), test=test)
+        return response.parse(FansitesSectionParser.from_content)
+
     # endregion
 
     # region Forums
     async def fetch_forum_section(
             self,
             section_id: int,
             *,
```

### Comparing `tibia.py-6.1.0/tibiapy/enums.py` & `tibia.py-6.2.0/tibiapy/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Enumerations used by models throughout the library."""
 from __future__ import annotations
 
 from enum import Enum, Flag, IntEnum
-from typing import Any, TYPE_CHECKING
+from typing import Any, Optional, TYPE_CHECKING
 
 from pydantic_core import core_schema
+from typing_extensions import Self
 
 from tibiapy.errors import EnumValueError
 from tibiapy.utils import try_enum
 
 if TYPE_CHECKING:
     from pydantic import GetCoreSchemaHandler, GetJsonSchemaHandler
     from pydantic.json_schema import JsonSchemaValue
@@ -47,15 +48,15 @@
     "WorldLocation",
 )
 
 
 class StringEnum(str, Enum):
 
     @classmethod
-    def validate(cls, v):
+    def validate(cls, v: Any) -> Self:
         e = try_enum(cls, v)
         if e is None:
             raise EnumValueError(cls, v)
 
         return e
 
     @classmethod
@@ -72,15 +73,15 @@
 
 
 class NumericEnum(IntEnum):
     def __str__(self):
         return self.name.lower()
 
     @classmethod
-    def validate(cls, v):
+    def validate(cls, v: Any):
         e = try_enum(cls, v)
         if e is None:
             raise EnumValueError(cls, v)
 
         return e
 
     @classmethod
@@ -244,15 +245,15 @@
 class BazaarType(StringEnum):
     """The possible bazaar types."""
 
     CURRENT = "Current Auctions"
     HISTORY = "Auction History"
 
     @property
-    def subtopic(self):
+    def subtopic(self) -> str:
         """The subtopic argument for this Bazaar type."""
         return "currentcharactertrades" if self == self.CURRENT else "pastcharactertrades"
 
 
 class BidType(StringEnum):
     """The possible bid types for an auction."""
 
@@ -319,15 +320,15 @@
     NONE = 1
     KNIGHTS = 2
     PALADINS = 3
     SORCERERS = 4
     DRUIDS = 5
 
     @classmethod
-    def from_name(cls, name, all_fallback=True):
+    def from_name(cls, name: str, all_fallback: bool = True) -> Optional[Self]:
         """Get a vocation filter from a vocation's name.
 
         Parameters
         ----------
         name: :class:`str`
             The name of the vocation.
         all_fallback: :class:`bool`
@@ -369,60 +370,60 @@
 class HouseType(StringEnum):
     """The types of house available."""
 
     HOUSE = "house"
     GUILDHALL = "guildhall"
 
     @property
-    def plural(self):
+    def plural(self) -> str:
         """:class:`str`: The plural for the house type."""
         return f"{self.value}s"
 
 
 class NewsCategory(StringEnum):
     """The different news categories."""
 
     CIPSOFT = "cipsoft"
     COMMUNITY = "community"
     DEVELOPMENT = "development"
     SUPPORT = "support"
     TECHNICAL_ISSUES = "technical"
 
     @property
-    def filter_name(self):
+    def filter_name(self) -> str:
         """The name of the filter parameter for this value."""
         return f"filter_{self.value}"
 
     @property
-    def big_icon_url(self):
+    def big_icon_url(self) -> str:
         """The URL to the big icon representing this category."""
         from tibiapy.urls import get_static_file_url
         return get_static_file_url("images", "global", "content", f"newsicon_{self.value}_big.gif")
 
     @property
-    def small_icon_url(self):
+    def small_icon_url(self) -> str:
         """The URL to the small icon representing this category."""
         from tibiapy.urls import get_static_file_url
         return get_static_file_url("images", "global", "content", f"newsicon_{self.value}_small.gif")
 
 
 class NewsType(StringEnum):
     """The different types of new entries."""
 
     NEWS_TICKER = "News Ticker"
     FEATURED_ARTICLE = "Featured Article"
     NEWS = "News"
 
     @property
-    def filter_name(self):
+    def filter_name(self) -> str:
         """The filter parameter name for this value."""
         return f"filter_{self.value.split(' ')[-1].lower()}"
 
     @property
-    def filter_value(self):
+    def filter_value(self) -> str:
         """The filter parameter value for this value."""
         return self.value.split(" ")[-1].lower()
 
 
 class PvpType(StringEnum):
     """The possible PvP types a World can have."""
 
@@ -495,30 +496,30 @@
         return ", ".join(v.name.title() for v in list(self))
 
     def __iter__(self):
         for entry in list(self.__class__):
             if entry in self and entry is not self.NONE:
                 yield entry
 
-    def get_icon_name(self):
+    def get_icon_name(self) -> Optional[str]:
         """Generate an icon name, following the same ordering used in Tibia.com.
 
         Returns
         -------
         :class:`str`
             The name of the icon used in Tibia.com
         """
         if self.value == 0:
             return None
 
         joined_str = "".join(v.name.lower() for v in list(self))
         return f"logo_{joined_str}.gif"
 
     @classmethod
-    def from_icon(cls, icon):
+    def from_icon(cls, icon: str) -> Self:
         """Get the flag combination, based from the icon's name present in the thread status.
 
         Parameters
         ----------
         icon: :class:`str`
             The icon's filename.
 
@@ -553,15 +554,15 @@
     SORCERER = "Sorcerer"
     ELDER_DRUID = "Elder Druid"
     ELITE_KNIGHT = "Elite Knight"
     ROYAL_PALADIN = "Royal Paladin"
     MASTER_SORCERER = "Master Sorcerer"
 
     @property
-    def base(self):
+    def base(self) -> Self:
         """The base vocation of this vocation if promoted. If not promoted, the same value is returned."""
         if self == self.ELDER_DRUID:
             return self.DRUID
         if self == self.MASTER_SORCERER:
             return self.SORCERER
         if self == self.ROYAL_PALADIN:
             return self.PALADIN
```

### Comparing `tibia.py-6.1.0/tibiapy/errors.py` & `tibia.py-6.2.0/tibiapy/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     Attributes
     ----------
     original: :class:`Exception`
         The original exception that caused this exception.
     """
 
-    def __init__(self, message, original=None):
+    def __init__(self, message: str, original=None):
         super().__init__(message)
         self.original = original
 
 
 @deprecated("Renamed to InvalidContentError")
 class InvalidContent(InvalidContentError):  # noqa: N818
     """Deprecated, use InvalidContentError instead."""
```

### Comparing `tibia.py-6.1.0/tibiapy/models/__init__.py` & `tibia.py-6.2.0/tibiapy/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from tibiapy.models.base import *
 from tibiapy.models.pagination import *
 from tibiapy.models.bazaar import *
 from tibiapy.models.character import *
 from tibiapy.models.creature import *
 from tibiapy.models.event import *
+from tibiapy.models.fansite import *
 from tibiapy.models.forum import *
 from tibiapy.models.guild import *
 from tibiapy.models.highscores import *
 from tibiapy.models.house import *
 from tibiapy.models.kill_statistics import *
 from tibiapy.models.leaderboard import *
 from tibiapy.models.news import *
```

### Comparing `tibia.py-6.1.0/tibiapy/models/base.py` & `tibia.py-6.2.0/tibiapy/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Base classes shared by various models."""
 from __future__ import annotations
 
+from typing import Any
+
 import pydantic
 from pydantic import ConfigDict
 
 import tibiapy
 
 __all__ = (
     "BaseModel",
@@ -69,15 +71,15 @@
     - :class:`.GuildMembership`
     - :class:`.GuildEntry`
     """
 
     name: str
     """The name of the guild."""
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any):
         if isinstance(other, self.__class__):
             return self.name == other.name
 
         return False
 
     @property
     def url(self) -> str:
```

### Comparing `tibia.py-6.1.0/tibiapy/models/bazaar.py` & `tibia.py-6.2.0/tibiapy/models/bazaar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Models relatd to the character bazaar."""
 import datetime
 from abc import ABC, abstractmethod
-from typing import Optional, List, Dict, TypeVar, Generic
+from typing import Dict, Generic, List, Optional, TypeVar
 
-from tibiapy.enums import (PvpTypeFilter, AuctionBattlEyeFilter, AuctionVocationFilter, AuctionSkillFilter,
-                           AuctionSearchType,
-                     AuctionOrderBy, AuctionOrderDirection, BazaarType, Vocation, Sex, BidType, AuctionStatus)
+from tibiapy.enums import (AuctionBattlEyeFilter, AuctionOrderBy, AuctionOrderDirection, AuctionSearchType,
+                           AuctionSkillFilter, AuctionStatus, AuctionVocationFilter, BazaarType, BidType, PvpTypeFilter,
+                           Sex, Vocation)
 from tibiapy.models import BaseModel
 from tibiapy.models.pagination import AjaxPaginator, PaginatedWithUrl
 
 __all__ = (
     "AchievementEntry",
     "Auction",
     "AuctionDetails",
@@ -23,14 +23,15 @@
     "ItemEntry",
     "ItemSummary",
     "MountEntry",
     "Mounts",
     "OutfitEntry",
     "OutfitImage",
     "Outfits",
+    "RevealedGem",
     "SalesArgument",
     "SkillEntry",
 )
 
 from tibiapy.urls import get_auction_url, get_bazaar_url, get_character_url
 
 
@@ -177,15 +178,15 @@
     name: str
     """The mount's name."""
     mount_id: int
     """The internal ID of the mount."""
 
 
 class OutfitEntry(DisplayImage, BaseOutfit):
-    """Represents a outfit owned or unlocked by the character."""
+    """Represents an outfit owned or unlocked by the character."""
 
     image_url: str
     """The URL to the image."""
     name: str
     """The outfit's name."""
     outfit_id: int
     """The internal ID of the outfit."""
@@ -213,30 +214,30 @@
     """The addons displayed in the outfit."""
 
 
 T = TypeVar("T", bound=DisplayImage)
 
 
 class AuctionSummary(AjaxPaginator[T], Generic[T], ABC):
-    def get_by_name(self, name):
+    def get_by_name(self, name: str):
         """Get an entry by its name.
 
         Parameters
         ----------
         name: :class:`str`
-            The name of the entry, case insensitive.
+            The name of the entry, case-insensitive.
 
         Returns
         -------
         :class:`object`:
             The entry matching the name.
         """
         return next((e for e in self.entries if e.name.lower() == name.lower()), None)
 
-    def search(self, value):
+    def search(self, value: str):
         """Search an entry by its name.
 
         Parameters
         ----------
         value: :class:`str`
             The value to look for.
 
@@ -244,22 +245,22 @@
         -------
         :class:`list`
             A list of entries with names containing the search term.
         """
         return [e for e in self.entries if value.lower() in e.name.lower()]
 
     @abstractmethod
-    def get_by_id(self, name):
+    def get_by_id(self, entry_id: int):
         ...
 
 
 class ItemSummary(AuctionSummary[ItemEntry]):
     """Items in a character's inventory and depot."""
 
-    def get_by_id(self, entry_id):
+    def get_by_id(self, entry_id: int) -> Optional[ItemEntry]:
         """Get an item by its item id.
 
         Parameters
         ----------
         entry_id: :class:`int`
             The ID of the item.
 
@@ -270,15 +271,15 @@
         """
         return next((e for e in self.entries if e.item_id == entry_id), None)
 
 
 class Mounts(AuctionSummary[MountEntry]):
     """The mounts the character has unlocked or purchased."""
 
-    def get_by_id(self, entry_id):
+    def get_by_id(self, entry_id: int) -> Optional[MountEntry]:
         """Get a mount by its mount id.
 
         Parameters
         ----------
         entry_id: :class:`int`
             The ID of the mount.
 
@@ -289,16 +290,16 @@
         """
         return next((e for e in self.entries if e.mount_id == entry_id), None)
 
 
 class Familiars(AuctionSummary[FamiliarEntry]):
     """The familiars the character has unlocked or purchased."""
 
-    def get_by_id(self, entry_id):
-        """Get an familiar by its familiar id.
+    def get_by_id(self, entry_id: int) -> Optional[FamiliarEntry]:
+        """Get a familiar by its familiar id.
 
         Parameters
         ----------
         entry_id: :class:`int`
             The ID of the familiar.
 
         Returns
@@ -308,15 +309,15 @@
         """
         return next((e for e in self.entries if e.familiar_id == entry_id), None)
 
 
 class Outfits(AuctionSummary[OutfitEntry]):
     """The outfits the character has unlocked or purchased."""
 
-    def get_by_id(self, entry_id):
+    def get_by_id(self, entry_id: int) -> Optional[OutfitEntry]:
         """Get an outfit by its outfit id.
 
         Parameters
         ----------
         entry_id: :class:`int`
             The ID of the outfit.
 
@@ -350,14 +351,16 @@
     level: int
     """The current level."""
     progress: float
     """The percentage of progress for the next level."""
 
 
 class RevealedGem(BaseModel):
+    """A gem that has been revealed for the character."""
+
     gem_type: str
     """The type of gem."""
     mods: List[str]
     """The mods or effects the gem has."""
 
 
 class AuctionDetails(BaseModel):
@@ -521,15 +524,15 @@
     """Represents the char bazaar."""
 
     type: BazaarType
     """The type of auctions being displayed, either current or auction history."""
     filters: Optional[AuctionFilters] = None
     """The currently set filtering options."""
 
-    def get_page_url(self, page) -> str:
+    def get_page_url(self, page: int) -> str:
         """Get the URL to a given page of the bazaar.
 
         Parameters
         ----------
         page: :class:`int`
             The desired page.
```

### Comparing `tibia.py-6.1.0/tibiapy/models/character.py` & `tibia.py-6.2.0/tibiapy/models/character.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibiapy/models/creature.py` & `tibia.py-6.2.0/tibiapy/models/creature.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibiapy/models/event.py` & `tibia.py-6.2.0/tibiapy/models/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Models related to the event schedule calendar."""
 import datetime
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from tibiapy.models import BaseModel
 from tibiapy.urls import get_event_schedule_url
 
 
 class EventEntry(BaseModel):
     """Represents an event's entry in the calendar."""
@@ -21,15 +21,15 @@
     """The day the event ends.
 
     If the event is continuing on the next month, this will be :obj:`None`."""
 
     color: Optional[str] = None
     """The displayed color of the event."""
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any):
         return self.title == other.title
 
     @property
     def duration(self) -> int:
         """The number of days this event will be active for."""
         return (self.end_date - self.start_date + datetime.timedelta(days=1)).days if (
                 self.end_date and self.start_date
@@ -69,13 +69,13 @@
             The events that are active during the desired_date, if any.
 
         Notes
         -----
         Dates outside the calendar's month and year may yield unexpected results.
         """
 
-        def is_between(start, end, desired_date):
+        def is_between(start: Optional[datetime.date], end: Optional[datetime.date], desired_date: datetime.date):
             start = start or datetime.date.min
             end = end or datetime.date.max
             return start <= desired_date <= end
 
         return [e for e in self.events if is_between(e.start_date, e.end_date, date)]
```

### Comparing `tibia.py-6.1.0/tibiapy/models/forum.py` & `tibia.py-6.2.0/tibiapy/models/forum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Models related to the forums."""
 import datetime
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from tibiapy.enums import ThreadStatus, Vocation
 from tibiapy.models import GuildMembership
 from tibiapy.models.base import BaseCharacter, BaseModel
 from tibiapy.models.pagination import PaginatedWithUrl
 from tibiapy.urls import (get_character_url, get_cm_post_archive_url, get_forum_announcement_url, get_forum_board_url,
                           get_forum_post_url, get_forum_section_url, get_forum_thread_url)
@@ -40,15 +40,15 @@
     - :class:`.ForumAnnouncement`
     - :class:`.AnnouncementEntry`
     """
 
     announcement_id: int
     """The ID of the announcement."""
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any):
         if isinstance(other, self.__class__):
             return other.announcement_id == self.announcement_id
 
         return False
 
     @property
     def url(self) -> str:
@@ -89,15 +89,15 @@
     - :class:`.ForumPost`
     - :class:`.LastPost`
     """
 
     post_id: int
     """The internal ID of the post."""
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any):
         if isinstance(other, self.__class__):
             return self.post_id == other.post_id
 
         return False
 
     @property
     def url(self) -> str:
@@ -114,19 +114,19 @@
     - :class:`.ForumThread`
     """
 
     thread_id: int
     """The internal ID of the thread."""
 
     @property
-    def url(self):
+    def url(self) -> str:
         """:class:`str`: The URL to the thread in Tibia.com."""
         return get_forum_thread_url(self.thread_id)
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any):
         if isinstance(other, self.__class__):
             return self.thread_id == other.thread_id
 
         return False
 
 
 class CMPost(BasePost):
@@ -156,15 +156,15 @@
     """The list of posts for the selected range."""
 
     @property
     def url(self) -> str:
         """The URL of the CM Post Archive with the current parameters."""
         return get_cm_post_archive_url(self.from_date, self.to_date, self.current_page)
 
-    def get_page_url(self, page) -> str:
+    def get_page_url(self, page: int) -> str:
         """Get the URL of the CM Post Archive at a specific page, with the current date parameters.
 
         Parameters
         ----------
         page: :class:`int`
             The desired page.
 
@@ -269,15 +269,15 @@
 
     section_id: int
     """The internal ID of the section."""
     entries: List[BoardEntry]
     """The boards in the forum section."""
 
     @property
-    def url(self):
+    def url(self) -> str:
         """The URL to this forum section."""
         return get_forum_section_url(self.section_id)
 
 
 class ThreadEntry(BaseThread):
     """Represents a thread in a forum board."""
 
@@ -354,15 +354,15 @@
 
     -1 means all threads will be shown."""
     announcements: List[AnnouncementEntry]
     """The list of announcements currently visible."""
     entries: List[ThreadEntry]
     """The list of threads currently visible."""
 
-    def get_page_url(self, page):
+    def get_page_url(self, page: int) -> str:
         """Get the URL to a given page of the board.
 
         Parameters
         ----------
         page: :class:`int`
             The desired page.
 
@@ -437,15 +437,15 @@
         return get_forum_thread_url(self.previous_topic_number) if self.previous_topic_number else None
 
     @property
     def next_thread_url(self) -> str:
         """The URL to the next topic of the board, if there's any."""
         return get_forum_thread_url(self.next_topic_number) if self.next_topic_number else None
 
-    def get_page_url(self, page):
+    def get_page_url(self, page: int) -> str:
         """Get the URL to a given page of the board.
 
         Parameters
         ----------
         page: :class:`int`
             The desired page.
```

### Comparing `tibia.py-6.1.0/tibiapy/models/guild.py` & `tibia.py-6.2.0/tibiapy/models/guild.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibiapy/models/highscores.py` & `tibia.py-6.2.0/tibiapy/models/highscores.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibiapy/models/house.py` & `tibia.py-6.2.0/tibiapy/models/house.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibiapy/models/kill_statistics.py` & `tibia.py-6.2.0/tibiapy/models/kill_statistics.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibiapy/models/leaderboard.py` & `tibia.py-6.2.0/tibiapy/models/leaderboard.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Models related to the leaderboards."""
 import datetime
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from tibiapy.models import BaseModel
 from tibiapy.models.pagination import PaginatedWithUrl
 from tibiapy.urls import get_leaderboards_url, get_character_url
 
 __all__ = (
     "LeaderboardEntry",
@@ -35,15 +35,15 @@
     rotation_id: int
     """The internal ID of the rotation."""
     is_current: bool
     """Whether this is the currently running rotation or not."""
     end_date: datetime.datetime
     """The date and time when this rotation ends."""
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any):
         if isinstance(other, self.__class__):
             return other.rotation_id == self.rotation_id
 
         return False
 
 
 class Leaderboard(PaginatedWithUrl[LeaderboardEntry]):
@@ -64,15 +64,15 @@
     """
 
     @property
     def url(self) -> str:
         """The URL to the current leaderboard."""
         return get_leaderboards_url(self.world, self.rotation.rotation_id, self.current_page)
 
-    def get_page_url(self, page):
+    def get_page_url(self, page: int) -> str:
         """Get the URL of the leaderboard at a specific page, with the current date parameters.
 
         Parameters
         ----------
         page: :class:`int`
             The desired page.
```

### Comparing `tibia.py-6.1.0/tibiapy/models/news.py` & `tibia.py-6.2.0/tibiapy/models/news.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibiapy/models/pagination.py` & `tibia.py-6.2.0/tibiapy/models/pagination.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     @property
     def previous_page_url(self) -> Optional[str]:
         """The URL to the previous page of the results, if available."""
         return None if self.current_page == 1 else self.get_page_url(self.current_page - 1)
 
     @abstractmethod
-    def get_page_url(self, page) -> str:
+    def get_page_url(self, page: int) -> str:
         """Get the URL to a specific page of the results."""
         ...
 
 
 class AjaxPaginator(Paginated[T], Generic[T]):
     """A paginator that can be fetched via AJAX requests."""
```

### Comparing `tibia.py-6.1.0/tibiapy/models/spell.py` & `tibia.py-6.2.0/tibiapy/models/spell.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibiapy/models/tibia_response.py` & `tibia.py-6.2.0/tibiapy/models/tibia_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Models used to wrap responses from Tibia.com."""
 import datetime
 from typing import Generic, TypeVar
 
 from pydantic import computed_field
+from typing_extensions import Self
 
 from tibiapy.models.base import BaseModel
 
 __all__ = (
     "TibiaResponse",
 )
 
@@ -37,20 +38,20 @@
     @property
     def time_left(self) -> datetime.timedelta:
         """:class:`datetime.timedelta`: The time left for the cache of this response to expire."""
         return (datetime.timedelta(seconds=CACHE_LIMIT - self.age)
                 - (datetime.datetime.now(datetime.timezone.utc) - self.timestamp))
 
     @property
-    def seconds_left(self):
+    def seconds_left(self) -> int:
         """:class:`int`: The time left in seconds for this response's cache to expire."""
         return self.time_left.seconds
 
     @classmethod
-    def from_raw(cls, raw_response, data: T, parsing_time=None):
+    def from_raw(cls, raw_response, data: T, parsing_time: float = None) -> Self:
         """Build an instance from a raw response."""
         return cls(
             timestamp=raw_response.timestamp,
             cached=raw_response.cached,
             age=raw_response.age,
             fetching_time=raw_response.fetching_time,
             parsing_time=parsing_time,
```

### Comparing `tibia.py-6.1.0/tibiapy/models/world.py` & `tibia.py-6.2.0/tibiapy/models/world.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         return int(self.creation_date.split("-")[1]) if self.creation_date else None
 
 
 class WorldEntry(BaseWorld):
     """Represents a game server listed in the World Overview section."""
 
 
-
 class WorldOverview(BaseModel):
     """Container class for the World Overview section."""
 
     record_count: int
     """The overall player online record."""
     record_date: datetime.datetime
     """The date when the record was achieved."""
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/bazaar.py` & `tibia.py-6.2.0/tibiapy/parsers/bazaar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Contains all classes related to the Character Bazaar sections in Tibia.com."""
 import logging
 import re
 import urllib.parse
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
 import bs4
 
 from tibiapy import InvalidContentError
 from tibiapy.builders import AuctionBuilder, AuctionDetailsBuilder, CharacterBazaarBuilder
 from tibiapy.enums import AuctionBattlEyeFilter, AuctionOrderBy, AuctionOrderDirection, AuctionSearchType, \
     AuctionSkillFilter, AuctionStatus, AuctionVocationFilter, BazaarType, BidType, PvpTypeFilter, Sex, Vocation
 from tibiapy.models import (AchievementEntry, AjaxPaginator, Auction, AuctionFilters, BestiaryEntry, BlessingEntry,
                             CharacterBazaar, CharmEntry, FamiliarEntry, Familiars, ItemEntry, ItemSummary, MountEntry,
                             Mounts, OutfitEntry, OutfitImage, Outfits, SalesArgument, SkillEntry)
-from tibiapy.models.bazaar import RevealedGem
+from tibiapy.models.bazaar import DisplayImage, RevealedGem
 from tibiapy.utils import (clean_text, convert_line_breaks, get_rows, parse_form_data, parse_integer, parse_pagination,
                            parse_tibia_datetime, parse_tibiacom_content, try_enum)
 
+CSS_CLASS_ICON = "div.CVIcon"
+
 results_pattern = re.compile(r"Results: (\d+)")
 char_info_regex = re.compile(r"Level: (\d+) \| Vocation: ([\w\s]+)\| (\w+) \| World: (\w+)")
 id_addon_regex = re.compile(r"(\d{1,4})_(\d)\.gif$")
 id_regex = re.compile(r"(\d{1,5}).(?:gif|png)$")
 description_regex = re.compile(r'"(?:an?\s)?([^"]+)"')
 amount_regex = re.compile(r"([\d,]{1,9})x")
 tier_regex = re.compile(r"(.*)\s\(tier (\d)\)")
@@ -220,15 +222,15 @@
         if "RevealedGems" in details_tables:
             cls._parse_revealed_gems_table(builder, details_tables["RevealedGems"])
 
         auction.details = builder.build()
         return auction
 
     @classmethod
-    def _parse_auction(cls, auction_row: bs4.Tag, auction_id=0) -> Auction:
+    def _parse_auction(cls, auction_row: bs4.Tag, auction_id: int = 0) -> Auction:
         """Parse an auction's table, extracting its data.
 
         Parameters
         ----------
         auction_row: :class:`bs4.Tag`
             The row containing the auction's information.
         auction_id: :class:`int`
@@ -257,15 +259,15 @@
             builder.sex(try_enum(Sex, m.group(3).strip().lower()))
             builder.world(m.group(4))
 
         outfit_img = auction_row.select_one("img.AuctionOutfitImage")
         if m := id_addon_regex.search(outfit_img["src"]):
             builder.outfit(OutfitImage(image_url=outfit_img["src"], outfit_id=int(m.group(1)), addons=int(m.group(2))))
 
-        item_boxes = auction_row.select("div.CVIcon")
+        item_boxes = auction_row.select(CSS_CLASS_ICON)
         for item_box in item_boxes:
             if item := cls._parse_displayed_item(item_box):
                 builder.add_displayed_item(item)
 
         dates_containers = auction_row.select_one("div.ShortAuctionData")
         start_date_tag, end_date_tag, *_ = dates_containers.select("div.ShortAuctionDataValue")
         builder.auction_start(parse_tibia_datetime(clean_text(start_date_tag)))
@@ -335,15 +337,15 @@
             value = row.select_one("div").text
             name = name.lower().strip().replace(" ", "_").replace(":", "")
             data[name] = value
 
         return data
 
     @classmethod
-    def _parse_skills_table(cls, builder: AuctionDetailsBuilder, table):
+    def _parse_skills_table(cls, builder: AuctionDetailsBuilder, table: bs4.Tag) -> None:
         """Parse the skills' table.
 
         Parameters
         ----------
         builder: :class:`AuctionDetailsBuilder`
             The builder where data will be stored to.
         table: :class:`bs4.Tag`
@@ -357,15 +359,15 @@
             level = int(level_c)
             progress = float(progress_c.replace("%", ""))
             skills.append(SkillEntry(name=name_c, level=level, progress=progress))
 
         builder.skills(skills)
 
     @classmethod
-    def _parse_blessings_table(cls, builder: AuctionDetailsBuilder, table):
+    def _parse_blessings_table(cls, builder: AuctionDetailsBuilder, table: bs4.Tag) -> None:
         """Parse the blessings table.
 
         Parameters
         ----------
         builder: :class:`AuctionDetailsBuilder`
             The builder where data will be stored to.
         table: :class:`bs4.Tag`
@@ -379,15 +381,15 @@
             amount_c, name_c = (c.text for c in cols)
             amount = int(amount_c.replace("x", ""))
             blessings.append(BlessingEntry(name=name_c, amount=amount))
 
         builder.blessings(blessings)
 
     @classmethod
-    def _parse_single_column_table(cls, table: bs4.Tag):
+    def _parse_single_column_table(cls, table: bs4.Tag) -> List[str]:
         """Parse a table with a single column into an array.
 
         Parameters
         ----------
         table: :class:`bs4.Tag`
             A table with a single column.
 
@@ -406,15 +408,15 @@
                 continue
 
             ret.append(text)
 
         return ret
 
     @classmethod
-    def _parse_charms_table(cls, builder: AuctionDetailsBuilder, table):
+    def _parse_charms_table(cls, builder: AuctionDetailsBuilder, table: bs4.Tag) -> None:
         """Parse the charms' table and extracts its information.
 
         Parameters
         ----------
         builder: :class:`AuctionDetailsBuilder`
             The builder where data will be stored to.
         table: :class:`bs4.Tag`
@@ -431,15 +433,15 @@
             cost_c, name_c = (c.text for c in cols)
             cost = parse_integer(cost_c.replace("x", ""))
             charms.append(CharmEntry(name=name_c, cost=cost))
 
         builder.charms(charms)
 
     @classmethod
-    def _parse_achievements_table(cls, builder: AuctionDetailsBuilder, table: bs4.Tag):
+    def _parse_achievements_table(cls, builder: AuctionDetailsBuilder, table: bs4.Tag) -> None:
         """Parse the achievements' table and extracts its information.
 
         Parameters
         ----------
         builder: :class:`AuctionDetailsBuilder`
             The builder where data will be stored to.
         table: :class:`bs4.Tag`
@@ -456,15 +458,15 @@
 
             secret = col.select_one("img") is not None
             achievements.append(AchievementEntry(name=text, is_secret=secret))
 
         builder.achievements(achievements)
 
     @classmethod
-    def _parse_bestiary_table(cls, builder: AuctionDetailsBuilder, table: bs4.Tag, bosstiary=False):
+    def _parse_bestiary_table(cls, builder: AuctionDetailsBuilder, table: bs4.Tag, bosstiary: bool = False) -> None:
         """Parse the bestiary table and extracts its information.
 
         Parameters
         ----------
         builder: :class:`AuctionDetailsBuilder`
             The builder where data will be stored to.
         table: :class:`bs4.Tag`
@@ -487,15 +489,15 @@
 
         if bosstiary:
             builder.bosstiary_progress(bestiary)
         else:
             builder.bestiary_progress(bestiary)
 
     @classmethod
-    def _parse_general_table(cls, builder: AuctionDetailsBuilder, table):
+    def _parse_general_table(cls, builder: AuctionDetailsBuilder, table: bs4.Tag) -> None:
         """Parse the general information table and assigns its values.
 
         Parameters
         ----------
         builder: :class:`AuctionDetailsBuilder`
             The builder where data will be stored to.
         table: :class:`bs4.Tag`
@@ -555,75 +557,75 @@
             builder.boss_points(parse_integer(boss_data.get("boss_points", "")))
 
         if len(content_containers) >= 11:
             bonus_promotion_data = cls._parse_data_table(content_containers[10])
             builder.bonus_promotion_points(parse_integer(bonus_promotion_data.get("bonus_promotion_points", "")))
 
     @classmethod
-    def _parse_items_table(cls, table: bs4.Tag):
+    def _parse_items_table(cls, table: bs4.Tag) -> ItemSummary:
         if pagination_block := table.select_one("div.BlockPageNavigationRow"):
             page, total_pages, results = parse_pagination(pagination_block)
         else:
             return ItemSummary()
 
         summary = ItemSummary(current_page=page, total_pages=total_pages, results_count=results)
-        item_boxes = table.select("div.CVIcon")
+        item_boxes = table.select(CSS_CLASS_ICON)
         for item_box in item_boxes:
             if item := cls._parse_displayed_item(item_box):
                 summary.entries.append(item)
 
         return summary
 
     @classmethod
-    def _parse_mounts_table(cls, table):
+    def _parse_mounts_table(cls, table: bs4.Tag) -> Mounts:
         if pagination_block := table.select_one("div.BlockPageNavigationRow"):
             page, total_pages, results = parse_pagination(pagination_block)
         else:
             return Mounts()
 
         summary = Mounts(current_page=page, total_pages=total_pages, results_count=results)
-        mount_boxes = table.select("div.CVIcon")
+        mount_boxes = table.select(CSS_CLASS_ICON)
         for mount_box in mount_boxes:
             if mount := cls._parse_displayed_mount(mount_box):
                 summary.entries.append(mount)
 
         return summary
 
     @classmethod
-    def _parse_outfits_table(cls, table):
+    def _parse_outfits_table(cls, table: bs4.Tag) -> Outfits:
         if pagination_block := table.select_one("div.BlockPageNavigationRow"):
             page, total_pages, results = parse_pagination(pagination_block)
         else:
             return Outfits()
 
         summary = Outfits(current_page=page, total_pages=total_pages, results_count=results)
-        outfit_boxes = table.select("div.CVIcon")
+        outfit_boxes = table.select(CSS_CLASS_ICON)
         for outfit_box in outfit_boxes:
             if outfit := cls._parse_displayed_outfit(outfit_box):
                 summary.entries.append(outfit)
 
         return summary
 
     @classmethod
-    def _parse_familiars_table(cls, table):
+    def _parse_familiars_table(cls, table: bs4.Tag) -> Familiars:
         if pagination_block := table.select_one("div.BlockPageNavigationRow"):
             page, total_pages, results = parse_pagination(pagination_block)
         else:
             return Familiars()
 
         summary = Familiars(current_page=page, total_pages=total_pages, results_count=results)
-        familiar_boxes = table.select("div.CVIcon")
+        familiar_boxes = table.select(CSS_CLASS_ICON)
         for familiar_box in familiar_boxes:
             if familiar := cls._parse_displayed_familiar(familiar_box):
                 summary.entries.append(familiar)
 
         return summary
 
     @classmethod
-    def _parse_displayed_item(cls, item_box):
+    def _parse_displayed_item(cls, item_box: bs4.Tag) -> Optional[ItemEntry]:
         title_text = item_box["title"]
         img_tag = item_box.select_one("img")
         if not img_tag:
             return None
 
         m = amount_regex.match(title_text)
         amount = 1
@@ -639,28 +641,28 @@
             name = m.group(1)
 
         item_id = int(m.group(1)) if (m := id_regex.search(img_tag["src"])) else 0
         return ItemEntry(image_url=img_tag["src"], name=name, count=amount, item_id=item_id, description=description,
                          tier=tier)
 
     @classmethod
-    def _parse_displayed_mount(cls, item_box):
+    def _parse_displayed_mount(cls, item_box: bs4.Tag) -> Optional[MountEntry]:
         description = item_box["title"]
         img_tag = item_box.select_one("img")
         if not img_tag:
             return None
 
         mount = MountEntry(image_url=img_tag["src"], name=description, mount_id=0)
         if m := id_regex.search(mount.image_url):
             mount.mount_id = int(m.group(1))
 
         return mount
 
     @classmethod
-    def _parse_displayed_outfit(cls, item_box):
+    def _parse_displayed_outfit(cls, item_box: bs4.Tag) -> Optional[OutfitEntry]:
         description = item_box["title"]
         img_tag = item_box.select_one("img")
         if not img_tag:
             return None
 
         outfit = OutfitEntry(image_url=img_tag["src"], name=description, outfit_id=0, addons=0)
         name = outfit.name.split("(")[0].strip()
@@ -668,45 +670,45 @@
         if m := id_addon_regex.search(outfit.image_url):
             outfit.outfit_id = int(m.group(1))
             outfit.addons = int(m.group(2))
 
         return outfit
 
     @classmethod
-    def _parse_displayed_familiar(cls, item_box):
+    def _parse_displayed_familiar(cls, item_box: bs4.Tag) -> Optional[FamiliarEntry]:
         description = item_box["title"]
         img_tag = item_box.select_one("img")
         if not img_tag:
             return None
 
         familiar = FamiliarEntry(image_url=img_tag["src"], name=description, familiar_id=0)
         name = familiar.name.split("(")[0].strip()
         familiar.name = name
         if m := id_regex.search(familiar.image_url):
             familiar.familiar_id = int(m.group(1))
 
         return familiar
 
     @classmethod
-    def _parse_revealed_gems_table(cls, builder: AuctionDetailsBuilder, table: bs4.Tag):
+    def _parse_revealed_gems_table(cls, builder: AuctionDetailsBuilder, table: bs4.Tag) -> None:
         table_content = table.select_one("table.TableContent")
         _, *rows = get_rows(table_content)
         for row in rows:
             gem_tag = row.select_one("div.Gem")
             gem_type = gem_tag["title"]
             effects = [t.text for t in row.select("span")]
             builder.add_revealed_gem(RevealedGem(
                 gem_type=gem_type,
                 mods=effects,
             ))
 
     @classmethod
-    def _parse_page_items(cls, content, paginator: AjaxPaginator):
+    def _parse_page_items(cls, content: str, paginator: AjaxPaginator) -> List[DisplayImage]:
         parsed_content = parse_tibiacom_content(content, builder="html5lib")
-        item_boxes = parsed_content.select("div.CVIcon")
+        item_boxes = parsed_content.select(CSS_CLASS_ICON)
         entries = []
         for item_box in item_boxes:
             if isinstance(paginator, ItemSummary):
                 item = cls._parse_displayed_item(item_box)
             elif isinstance(paginator, Outfits):
                 item = cls._parse_displayed_outfit(item_box)
             elif isinstance(paginator, Mounts):
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/character.py` & `tibia.py-6.2.0/tibiapy/parsers/character.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             if title in table_parsers:
                 action = table_parsers[title]
                 action(table)
 
         return builder.build()
 
     @classmethod
-    def _parse_account_information(cls, builder: CharacterBuilder, rows: list[bs4.Tag]):
+    def _parse_account_information(cls, builder: CharacterBuilder, rows: list[bs4.Tag]) -> None:
         """Parse the character's account information."""
         acc_info = {}
 
         for row in rows:
             cols_raw = row.select("td")
             cols = [ele.text.strip() for ele in cols_raw]
             field, value = cols
@@ -107,15 +107,15 @@
 
         created = parse_tibia_datetime(acc_info["created"])
         loyalty_title = None if acc_info["loyalty_title"] == "(no title)" else acc_info["loyalty_title"]
         position = acc_info.get("position")
         builder.account_information(AccountInformation(created=created, loyalty_title=loyalty_title, position=position))
 
     @classmethod
-    def _parse_achievements(cls, builder: CharacterBuilder, rows: List[bs4.Tag]):
+    def _parse_achievements(cls, builder: CharacterBuilder, rows: List[bs4.Tag]) -> None:
         """Parse the character's displayed achievements."""
         for row in rows:
             cols = row.select("td")
             if len(cols) != 2:
                 continue
 
             field, value = cols
@@ -123,29 +123,29 @@
             name = value.text.strip()
             secret_image = value.select_one("img")
             secret = secret_image is not None
 
             builder.add_achievement(Achievement(name=name, grade=grade, is_secret=secret))
 
     @classmethod
-    def _parse_account_badges(cls, builder: CharacterBuilder, rows: List[bs4.Tag]):
+    def _parse_account_badges(cls, builder: CharacterBuilder, rows: List[bs4.Tag]) -> None:
         """Parse the character's displayed badges."""
         row = rows[0]
         columns = row.select("td > span")
         for column in columns:
             popup_span = column.select_one("span.HelperDivIndicator")
             popup = parse_popup(popup_span["onmouseover"])
             name = popup[0]
             description = popup[1].text
             icon_image = column.select_one("img")
             icon_url = icon_image["src"]
             builder.add_account_badge(AccountBadge(name=name, icon_url=icon_url, description=description))
 
     @classmethod
-    def _parse_character_information(cls, builder: CharacterBuilder, rows: List[bs4.Tag]):
+    def _parse_character_information(cls, builder: CharacterBuilder, rows: List[bs4.Tag]) -> None:
         """Parse the character's basic information and applies the found values."""
         field_actions: dict[str, Callable[[bs4.Tag, str], None]] = {
             "name": lambda rv, v: cls._parse_name_field(builder, v),
             "title": lambda rv, v: cls._parse_titles(builder, v),
             "former names": lambda rv, v: builder.former_names([fn.strip() for fn in v.split(",")]),
             "former world": lambda rv, v: builder.former_world(v),
             "sex": lambda rv, v: builder.sex(try_enum(Sex, v)),
@@ -172,39 +172,39 @@
             if field in field_actions:
                 action = field_actions[field]
                 action(raw_value, value)
             else:
                 logger.debug("Unhandled character information field found: %s", field)
 
     @classmethod
-    def _parse_name_field(cls, builder: CharacterBuilder, value: str):
+    def _parse_name_field(cls, builder: CharacterBuilder, value: str) -> None:
         if m := deleted_regexp.match(value):
             value = m.group(1)
             builder.name(value)
             builder.deletion_date(parse_tibia_datetime(m.group(2)))
         else:
             builder.name(value)
 
         if traded_label in value:
             builder.name(value.replace(traded_label, "").strip())
             builder.traded(True)
 
     @classmethod
-    def _parse_titles(cls, builder: CharacterBuilder, value: str):
+    def _parse_titles(cls, builder: CharacterBuilder, value: str) -> None:
         if m := title_regexp.match(value):
             name = m.group(1).strip()
             unlocked = int(m.group(2))
             if name == "None":
                 name = None
 
             builder.title(name)
             builder.unlocked_titles(unlocked)
 
     @classmethod
-    def _parse_house_column(cls, builder: CharacterBuilder, column: bs4.Tag):
+    def _parse_house_column(cls, builder: CharacterBuilder, column: bs4.Tag) -> None:
         house_text = clean_text(column)
         m = house_regexp.search(house_text)
         paid_until = m.group(1)
         paid_until_date = parse_tibia_date(paid_until)
         house_link_tag = column.select_one("a")
         house_link = parse_link_info(house_link_tag)
         builder.add_house(
@@ -214,22 +214,22 @@
                 town=house_link["query"]["town"],
                 paid_until=paid_until_date,
                 world=house_link["query"]["world"],
             ),
         )
 
     @classmethod
-    def _parse_guild_column(cls, builder: CharacterBuilder, column: bs4.Tag):
+    def _parse_guild_column(cls, builder: CharacterBuilder, column: bs4.Tag) -> None:
         guild_link = column.select_one("a")
         value = clean_text(column)
         rank = value.split("of the")[0]
         builder.guild_membership(GuildMembership(name=clean_text(guild_link), rank=rank.strip()))
 
     @classmethod
-    def _parse_deaths(cls, builder: CharacterBuilder, rows: List[bs4.Tag]):
+    def _parse_deaths(cls, builder: CharacterBuilder, rows: List[bs4.Tag]) -> None:
         """Parse the character's recent deaths."""
         for row in rows:
             cols = row.select("td")
             if len(cols) != 2:
                 builder.deaths_truncated(True)
                 break
 
@@ -281,15 +281,15 @@
         if m := death_summon.search(name):
             summon = clean_text(m.group("summon"))
             name = clean_text(m.group("name"))
 
         return DeathParticipant(name=name, is_player=player, summon=summon, is_traded=traded)
 
     @classmethod
-    def _parse_other_characters(cls, builder: CharacterBuilder, rows: List[bs4.Tag]):
+    def _parse_other_characters(cls, builder: CharacterBuilder, rows: List[bs4.Tag]) -> None:
         """Parse the character's other visible characters."""
         for row in rows[1:]:
             cols_raw = row.select("td")
             cols = [ele.text.strip() for ele in cols_raw]
             if len(cols) != 4:
                 continue
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/creature.py` & `tibia.py-6.2.0/tibiapy/parsers/creature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Models related to the creatures section in the library."""
 import os
 import re
 import urllib.parse
-from typing import Optional
+from typing import List, Optional, Tuple
 
 import bs4
 
 from tibiapy.builders import CreatureBuilder
 from tibiapy.errors import InvalidContentError
 from tibiapy.models import CreatureEntry, CreaturesSection, BoostedCreatures, BossEntry, BoostableBosses, Creature
 from tibiapy.utils import parse_tibiacom_content, convert_line_breaks
@@ -29,15 +29,15 @@
 MANA_COST = re.compile(r"takes (\d+) mana")
 
 
 class BoostedCreaturesParser:
     """Parser for boosted creatures and bosses."""
 
     @classmethod
-    def _parse_boosted_platform(cls, parsed_content: bs4.BeautifulSoup, tag_id: str):
+    def _parse_boosted_platform(cls, parsed_content: bs4.BeautifulSoup, tag_id: str) -> Tuple[str, str]:
         img = parsed_content.select_one(f"#{tag_id}")
         name = BOOSTED_ALT.sub("", img["title"]).strip()
         image_url = img["src"]
         identifier = image_url.split("/")[-1].replace(".gif", "")
         return name, identifier
 
     @classmethod
@@ -224,15 +224,15 @@
 
         Returns
         -------
             The creature contained in the page.
         """
         try:
             parsed_content = parse_tibiacom_content(content)
-            pagination_container, content_container = (
+            _, content_container = (
                 parsed_content.find_all("div", style=lambda v: v and "position: relative" in v)
             )
             title_container, description_container = content_container.select("div")
             title = title_container.select_one("h2")
             name = title.text.strip()
 
             img = title_container.select_one("img")
@@ -250,15 +250,15 @@
             exp_text = paragraphs[-1]
             cls._parse_exp_text(builder, exp_text)
             return builder.build()
         except ValueError:
             return None
 
     @classmethod
-    def _parse_exp_text(cls, builder, exp_text):
+    def _parse_exp_text(cls, builder: CreatureBuilder, exp_text: str) -> None:
         """Parse the experience text, containing dropped loot and adds it to the creature.
 
         Parameters
         ----------
         builder: :class:`CreatureBuilder`
             The builder where data will be stored to.
         exp_text: :class:`str`
@@ -267,15 +267,15 @@
         if m := EXP_PATTERN.search(exp_text):
             builder.experience(int(m.group(1)))
 
         if m := LOOT_PATTERN.search(exp_text):
             builder.loot(m.group(1))
 
     @classmethod
-    def _parse_hp_text(cls, builder: CreatureBuilder, hp_text):
+    def _parse_hp_text(cls, builder: CreatureBuilder, hp_text: str) -> None:
         """Parse the text containing the creature's hitpoints, containing weaknesses, immunities and more and adds it.
 
         Parameters
         ----------
         builder: :class:`CreatureBuilder`
             The builder where data will be stored to.
         hp_text: :class:`str`
@@ -312,18 +312,16 @@
             if "cannot be summoned" in hp_text:
                 builder.convinceable(True)
 
             if "cannot be convinced" in hp_text:
                 builder.summonable(True)
 
     @classmethod
-    def _parse_elements(cls, text):
+    def _parse_elements(cls, text: str) -> List[str]:
         """Parse the elements found in a string, adding them to the collection.
 
         Parameters
         ----------
-        collection: :class:`list`
-            The collection where found elements will be added to.
         text: :class:`str`
             The text containing the elements.
         """
         return [element for element in cls._valid_elements if element in text]
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/event.py` & `tibia.py-6.2.0/tibiapy/parsers/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Models related to the event schedule section in Tibia.com."""
 
 import datetime
 import re
 import time
-from typing import List, Tuple
+from typing import Dict, List, Tuple
 
 import bs4
 
 from tibiapy.builders import EventScheduleBuilder
 from tibiapy.models import EventEntry, EventSchedule
 from tibiapy.utils import parse_popup, parse_tibiacom_content
 
@@ -101,15 +101,15 @@
             # Set to december of previous year
             month = 12
             year -= 1
 
         return month, year
 
     @classmethod
-    def _parse_inline_style(cls, style_content):
+    def _parse_inline_style(cls, style_content: str) -> Dict[str, str]:
         attrs = style_content.split(";")
         values = {}
         for attr in attrs:
             if not attr.strip():
                 continue
 
             key, value = attr.split(":")
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/forum.py` & `tibia.py-6.2.0/tibiapy/parsers/forum.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,20 @@
         return builder.build()
 
     # endregion
 
     # region Private Methods
 
     @classmethod
-    def _get_selected_date(cls, month_selector: bs4.Tag, day_selector: bs4.Tag, year_selector: bs4.Tag):
+    def _get_selected_date(
+            cls,
+            month_selector: bs4.Tag,
+            day_selector: bs4.Tag,
+            year_selector: bs4.Tag,
+    ) -> Optional[datetime.date]:
         """Get the date made from the selected options in the selectors.
 
         Parameters
         ----------
         month_selector: :class:`bs4.Tag`
             The month selector.
         day_selector: :class:`bs4.Tag`
@@ -171,15 +176,15 @@
         section_id = redirect_qs["sectionid"][0]
         time_label = parsed_content.select_one("div.CurrentTime")
         offset = 2 if "CEST" in time_label.text else 1
         boards = [board for row in rows if (board := cls._parse_board_row(row, offset)) is not None]
         return ForumSection(section_id=int(section_id), entries=boards)
 
     @classmethod
-    def _parse_board_row(cls, board_row, offset=1):
+    def _parse_board_row(cls, board_row: bs4.Tag, offset: int = 1) -> Optional[BoardEntry]:
         """Parse a row containing a board and extracts its information.
 
         Parameters
         ----------
         board_row: :class:`bs4.Tag`
             The row's parsed content.
         offset: :class:`int`
@@ -284,15 +289,15 @@
         builder.from_date(start_date).to_date(end_date)
         return builder.build()
 
 
 class ForumAuthorParser:
 
     @classmethod
-    def _parse_author_table(cls, character_info_container):
+    def _parse_author_table(cls, character_info_container: bs4.Tag) -> ForumAuthor:
         """Parse the table containing the author's information.
 
         Parameters
         ----------
         character_info_container: :class:`bs4.Tag`
             The cotnainer with the character's information.
 
@@ -435,15 +440,15 @@
         return builder.build()
 
     # endregion
 
     # region Private Methods
 
     @classmethod
-    def _parse_thread_row(cls, columns):
+    def _parse_thread_row(cls, columns: bs4.ResultSet) -> Optional[ThreadEntry]:
         """Parse the thread row, containing a single thread.
 
         Parameters
         ----------
         columns: :class:`bs4.ResultSet`
             The list of columns the thread contains.
 
@@ -609,15 +614,15 @@
         return builder.build()
 
     # endregion
 
     # region Private Methods
 
     @classmethod
-    def _parse_post_table(cls, post_table, offset=1):
+    def _parse_post_table(cls, post_table: bs4.Tag, offset: int = 1) -> ForumPost:
         """Parse the table containing a single posts, extracting its information.
 
         Parameters
         ----------
         post_table: :class:`bs4.Tag`
             The parsed HTML content of the table.
         offset: :class:`int`
@@ -689,15 +694,15 @@
 
     # endregion
 
 
 class LastPostParser:
 
     @classmethod
-    def _parse_column(cls, last_post_column, offset=1):
+    def _parse_column(cls, last_post_column: bs4.Tag, offset: int = 1) -> Optional[LastPost]:
         """Parse the column containing the last post information and extracts its data.
 
         Parameters
         ----------
         last_post_column: :class:`bs4.Tag`:
             The column containing the last post.
         offset: :class:`int`
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/guild.py` & `tibia.py-6.2.0/tibiapy/parsers/guild.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Models related to the guilds section in Tibia.com."""
 from __future__ import annotations
 
 import datetime
 import re
-from typing import Optional, TYPE_CHECKING
+from typing import Dict, Optional, TYPE_CHECKING, Tuple
 
 from tibiapy.builders import GuildBuilder, GuildWarEntryBuilder, GuildWarsBuilder
 from tibiapy.errors import InvalidContentError
 from tibiapy.models import GuildEntry, GuildHouse, GuildInvite, GuildMember, GuildWarEntry, GuildsSection
 from tibiapy.utils import clean_text, parse_form_data, parse_link_info, parse_tibia_date, parse_tibiacom_content
 
 if TYPE_CHECKING:
@@ -145,15 +145,20 @@
 
         return builder.build()
 
     # endregion
 
     # region Private methods
     @classmethod
-    def _parse_current_member(cls, builder, previous_rank, values):
+    def _parse_current_member(
+            cls,
+            builder: GuildBuilder,
+            previous_rank: Dict[int, str],
+            values: Tuple[str, ...],
+    ) -> None:
         """Parse the column texts of a member row into a member dictionary.
 
         Parameters
         ----------
         builder: :class:`GuildBuilder`
             The builder where data will be stored to.
         previous_rank: :class:`dict`[int, str]
@@ -170,15 +175,15 @@
             title = m.group(2)
 
         joined = parse_tibia_date(joined)
         builder.add_member(GuildMember(name=name.strip(), rank=rank.strip(), title=title, level=int(level),
                                        vocation=vocation, joined_on=joined, is_online=status == "online"))
 
     @classmethod
-    def _parse_application_info(cls, builder, info_container):
+    def _parse_application_info(cls, builder: GuildBuilder, info_container: bs4.Tag) -> None:
         """Parse the guild's application info.
 
         Parameters
         ----------
         builder: :class:`GuildBuilder`
             The builder where data will be stored to.
         info_container: :class:`bs4.Tag`
@@ -186,45 +191,45 @@
         """
         if m := applications_regex.search(info_container.text):
             builder.open_applications(m.group(1) == "opened")
 
         builder.active_war("during war" in info_container.text)
 
     @classmethod
-    def _parse_guild_disband_info(cls, builder: GuildBuilder, info_container: bs4.Tag):
+    def _parse_guild_disband_info(cls, builder: GuildBuilder, info_container: bs4.Tag) -> None:
         """Parse the guild's disband info, if available.
 
         Parameters
         ----------
         builder: :class:`GuildBuilder`
             The builder where data will be stored to.
         info_container: :class:`bs4.Tag`
             The parsed content of the information container.
         """
         if m := disband_regex.search(info_container.text):
             builder.disband_condition(m.group(2))
             builder.disband_date(parse_tibia_date(clean_text(m.group(1))))
 
     @classmethod
-    def _parse_guild_guildhall(cls, builder, info_container):
+    def _parse_guild_guildhall(cls, builder: GuildBuilder, info_container: bs4.Tag) -> None:
         """Parse the guild's guildhall info.
 
         Parameters
         ----------
         builder: :class:`GuildBuilder`
             The builder where data will be stored to.
         info_container: :class:`bs4.Tag`
             The parsed content of the information container.
         """
         if m := guildhall_regex.search(info_container.text):
             paid_until = parse_tibia_date(clean_text(m.group("date")))
             builder.guildhall(GuildHouse(name=m.group("name"), paid_until=paid_until))
 
     @classmethod
-    def _parse_guild_homepage(cls, builder, info_container):
+    def _parse_guild_homepage(cls, builder: GuildBuilder, info_container: bs4.Tag) -> None:
         """Parse the guild's homepage info.
 
         Parameters
         ----------
         builder: :class:`GuildBuilder`
             The builder where data will be stored to.
         info_container: :class:`bs4.Tag`
@@ -237,15 +242,15 @@
             link_info = parse_link_info(link)
             if "target" in link_info["query"]:
                 builder.homepage(link_info["query"]["target"])
             else:
                 builder.homepage(link_info["url"])
 
     @classmethod
-    def _parse_guild_info(cls, builder, info_container):
+    def _parse_guild_info(cls, builder: GuildBuilder, info_container: bs4.Tag) -> None:
         """Parse the guild's general information and applies the found values.
 
         Parameters
         ----------
         builder: :class:`GuildBuilder`
             The builder where data will be stored to.
         info_container: :class:`bs4.Tag`
@@ -255,15 +260,15 @@
             description = m.group("desc").strip()
             builder.description(description or None)
             builder.world(m.group("world"))
             builder.founded(parse_tibia_date(clean_text(m.group("date"))))
             builder.active("currently active" in m.group("status"))
 
     @classmethod
-    def _parse_logo(cls, builder: GuildBuilder, parsed_content):
+    def _parse_logo(cls, builder: GuildBuilder, parsed_content: bs4.Tag) -> bool:
         """Parse the guild logo and saves it to the instance.
 
         Parameters
         ----------
         builder: :class:`GuildBuilder`
             The builder where data will be stored to.
         parsed_content: :class:`bs4.Tag`
@@ -277,15 +282,15 @@
         logo_img = parsed_content.select_one('img[height="64"]')
         if logo_img is None:
             raise InvalidContentError("content does not belong to a Tibia.com guild page.")
 
         builder.logo_url(logo_img["src"])
 
     @classmethod
-    def _parse_guild_members(cls, builder, parsed_content):
+    def _parse_guild_members(cls, builder: GuildBuilder, parsed_content: bs4.Tag) -> None:
         """Parse the guild's member and invited list.
 
         Parameters
         ----------
         builder: :class:`GuildBuilder`
             The builder where data will be stored to.
         parsed_content: :class:`bs4.Tag`
@@ -299,15 +304,15 @@
             if len(columns) == COLS_GUILD_MEMBER:
                 cls._parse_current_member(builder, previous_rank, values)
 
             if len(columns) == COLS_INVITED_MEMBER:
                 cls._parse_invited_member(builder, values)
 
     @classmethod
-    def _parse_invited_member(cls, builder, values):
+    def _parse_invited_member(cls, builder: GuildBuilder, values: tuple[str, ...]) -> None:
         """Parse the column texts of an invited row into a invited dictionary.
 
         Parameters
         ----------
         builder: :class:`GuildBuilder`
             The builder where data will be stored to.
         values: tuple[:class:`str`]
@@ -369,15 +374,15 @@
                 builder.name(history_entries[0].guild_name)
 
             return builder.build()
         except ValueError as e:
             raise InvalidContentError("content does not belong to the guild wars section", e) from e
 
     @classmethod
-    def _parse_current_war_information(cls, text) -> GuildWarEntry:
+    def _parse_current_war_information(cls, text: str) -> GuildWarEntry:
         """Parse the guild's current war information.
 
         Parameters
         ----------
         text: :class:`str`
             The text describing the current war's information.
 
@@ -403,15 +408,15 @@
         end_date_match = war_end_regex.search(text)
         end_date_str = end_date_match.group(1)
         builder.end_date(parse_tibia_date(end_date_str))
 
         return builder.build()
 
     @classmethod
-    def _parse_war_history_entry(cls, text):
+    def _parse_war_history_entry(cls, text: str) -> GuildWarEntry:
         """Parse a guild's war information.
 
         Parameters
         ----------
         text: :class:`str`
             The text describing the war's information.
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/highscores.py` & `tibia.py-6.2.0/tibiapy/parsers/highscores.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibiapy/parsers/house.py` & `tibia.py-6.2.0/tibiapy/parsers/house.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,26 +100,26 @@
                 builder.add_entry(house_builder.build())
 
             return builder.build()
         except (ValueError, AttributeError, KeyError) as e:
             raise InvalidContentError("content does not belong to a Tibia.com house list", e) from e
 
     @classmethod
-    def _parse_filters(cls, builder: HousesSectionBuilder, form: bs4.Tag):
+    def _parse_filters(cls, builder: HousesSectionBuilder, form: bs4.Tag) -> None:
         form_data = parse_form_data(form)
         builder.available_worlds(list(form_data.available_options["world"].values()))
         builder.available_towns(list(form_data.available_options["town"].values()))
         builder.world(form_data.values["world"])
         builder.town(form_data.values["town"])
         builder.status(try_enum(HouseStatus, form_data.values.get("state")))
         builder.house_type(try_enum(HouseType, form_data.values.get("type", "")[:-1]))
         builder.order(try_enum(HouseOrder, form_data.values.get("order"), HouseOrder.NAME))
 
     @classmethod
-    def _parse_status(cls, builder: HouseEntryBuilder, status):
+    def _parse_status(cls, builder: HouseEntryBuilder, status: str) -> None:
         """Parse the status string found in the table and applies the corresponding values.
 
         Parameters
         ----------
         builder: :class:`HouseEntryBuilder`
             The instance of the builder where data will be collected.
         status: :class:`str`
@@ -199,15 +199,15 @@
             return builder.build()
         except (ValueError, TypeError) as e:
             raise InvalidContentError("content does not belong to a house page", e) from e
 
     # endregion
 
     @classmethod
-    def _parse_status(cls, builder: HouseBuilder, status):
+    def _parse_status(cls, builder: HouseBuilder, status: str) -> None:
         """Parse the house's state description and applies the corresponding values.
 
         Parameters
         ----------
         builder: :class:`HouseBuilder`
             The instance of the builder where data will be collected.
         status: :class:`str`
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/kill_statistics.py` & `tibia.py-6.2.0/tibiapy/parsers/kill_statistics.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.1.0/tibiapy/parsers/leaderboard.py` & `tibia.py-6.2.0/tibiapy/parsers/leaderboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             pages, total, count = parse_pagination(pagination_block) if pagination_block else (0, 0, 0)
             builder.current_page(pages).total_pages(total).results_count(count)
             return builder.build()
         except (AttributeError, ValueError, KeyError) as e:
             raise errors.InvalidContentError("content does not belong to the leaderboards", e) from e
 
     @classmethod
-    def _parse_entries(cls, builder: LeaderboardBuilder, entries_table: Tag):
+    def _parse_entries(cls, builder: LeaderboardBuilder, entries_table: Tag) -> None:
         entries_rows = entries_table.select("tr[style]")
         for row in entries_rows:
             columns = row.select("td")
             if len(columns) != 3:
                 continue
 
             rank = parse_integer(columns[0].text.replace(".", ""))
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/news.py` & `tibia.py-6.2.0/tibiapy/parsers/news.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Parsers for the news archive and news articles."""
 import datetime
 import re
 import urllib.parse
-from typing import Optional, Set, Dict, Union
+from typing import List, Optional, Set, Dict, Union
 
 import bs4
 
 from tibiapy.builders.news import NewsArchiveBuilder, NewsBuilder
 from tibiapy.enums import NewsCategory, NewsType
 from tibiapy.errors import InvalidContentError
 from tibiapy.models.news import NewsArchive, News, NewsEntry
@@ -113,15 +113,15 @@
                     continue
 
                 builder.add_entry(cls._parse_entry(cols_raw))
 
         return builder.build()
 
     @classmethod
-    def _parse_filter_table(cls, builder: NewsArchiveBuilder, form: bs4.Tag):
+    def _parse_filter_table(cls, builder: NewsArchiveBuilder, form: bs4.Tag) -> None:
         form_data = parse_form_data(form)
         builder.from_date(datetime.date(
             int(form_data.values["filter_begin_year"]),
             int(form_data.values["filter_begin_month"]),
             int(form_data.values["filter_begin_day"]),
         )).to_date(
             datetime.date(
@@ -135,15 +135,15 @@
                 builder.add_type(news_type)
 
         for category in NewsCategory:  # type: NewsCategory
             if category.filter_name in form_data.values_multiple:
                 builder.add_category(category)
 
     @classmethod
-    def _parse_entry(cls, cols_raw):
+    def _parse_entry(cls, cols_raw: List[bs4.Tag]) -> NewsEntry:
         img = cols_raw[0].select_one("img")
         img_url = img["src"]
         category_name = ICON_PATTERN.search(img_url)
         category = try_enum(NewsCategory, category_name.group(1))
         for br in cols_raw[1].select("br"):
             br.replace_with("\n")
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/spell.py` & `tibia.py-6.2.0/tibiapy/parsers/spell.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         builder.description(cls._parse_description(title_table))
         if "Rune Information" in tables:
             builder.rune(cls._parse_rune_table(tables["Rune Information"]))
 
         return builder.build()
 
     @classmethod
-    def _parse_description(cls, title_table):
+    def _parse_description(cls, title_table: bs4.Tag) -> str:
         next_sibling = title_table.next_sibling
         description = ""
         while next_sibling:
             if isinstance(next_sibling, bs4.Tag):
                 if next_sibling.name == "br":
                     description += "\n"
                 elif next_sibling.name in ["table", "div"]:
@@ -157,15 +157,15 @@
                 description += next_sibling.text
 
             next_sibling = next_sibling.next_sibling
 
         return description.strip()
 
     @classmethod
-    def _parse_rune_table(cls, table) -> Rune:
+    def _parse_rune_table(cls, table: bs4.Tag) -> Rune:
         """Parse the rune information table.
 
         Parameters
         ----------
         table: :class:`bs4.Tag`
             The table containing the rune information.
 
@@ -181,28 +181,23 @@
                 .magic_type(attrs.get("magic_type"))
                 .magic_level(parse_integer(attrs.get("mag_lvl"), 0))
                 .exp_level(parse_integer(attrs.get("exp_lvl"), 0))
                 .mana(parse_integer(attrs.get("mana"), None))
                 .build())
 
     @classmethod
-    def _parse_spells_table(cls, builder: SpellBuilder, spell_table: bs4.Tag):
+    def _parse_spells_table(cls, builder: SpellBuilder, spell_table: bs4.Tag) -> None:
         """Parse the table containing spell information.
 
         Parameters
         ----------
         builder: :class:`SpellBuilder`
             The instance of the builder where data will be collected.
         spell_table: :class:`bs4.Tag`
             The table containing the spell information.
-
-        Returns
-        -------
-        :class:`Spell`
-            The spell described in the table.
         """
         attrs = cls._parse_table_attributes(spell_table)
         builder.name(attrs["name"])
         builder.words(attrs["formula"])
         builder.is_premium("yes" in attrs["premium"])
         builder.exp_level(parse_integer(attrs["exp_lvl"], None))
         builder.vocations([s.strip() for s in attrs["vocation"].split(",")])
@@ -218,18 +213,17 @@
         builder.cooldown_group_secondary(parse_integer(cooldowns.get("secondary_group_cooldown"), None))
         builder.spell_type(try_enum(SpellType, attrs["type"]))
         builder.soul_points(parse_integer(attrs.get("soul_points"), None))
         builder.mana(parse_integer(attrs.get("mana"), None))
         builder.amount(parse_integer(attrs.get("amount"), None))
         builder.price(parse_integer(attrs.get("price"), 0))
         builder.magic_type(attrs.get("magic_type"))
-        return builder
 
     @classmethod
-    def _parse_table_attributes(cls, table) -> Dict[str, str]:
+    def _parse_table_attributes(cls, table: bs4.Tag) -> Dict[str, str]:
         """Parse the attributes of a table.
 
         Create a dictionary where every key is the left column (cleaned up) and the value is the right column.
 
         Parameters
         ----------
         table: :class:`bs4.Tag`
```

### Comparing `tibia.py-6.1.0/tibiapy/parsers/world.py` & `tibia.py-6.2.0/tibiapy/parsers/world.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         except AttributeError as e:
             raise InvalidContentError("content is not from the world section in Tibia.com") from e
 
         return builder.build()
 
     @classmethod
-    def _parse_world_info(cls, builder: WorldBuilder, world_info_table: bs4.Tag):
+    def _parse_world_info(cls, builder: WorldBuilder, world_info_table: bs4.Tag) -> None:
         """Parse the World Information table from Tibia.com and adds the found values to the object.
 
         Parameters
         ----------
         builder: :class:`WorldBuilder`
             The instance of the builder where data will be collected.
         world_info_table: :class:`bs4.Tag`
@@ -103,33 +103,33 @@
             field, value = cols
             field = field.replace(":", "")
             if field in field_actions:
                 action = field_actions[field]
                 action(value)
 
     @classmethod
-    def _parse_world_quest_titles(cls, builder: WorldBuilder, value: str):
+    def _parse_world_quest_titles(cls, builder: WorldBuilder, value: str) -> None:
         titles = [q.strip() for q in value.split(",")]
         if "currently has no title" not in titles[0]:
             builder.world_quest_titles(titles)
 
     @classmethod
-    def _parse_online_record(cls, builder: WorldBuilder, value: str):
+    def _parse_online_record(cls, builder: WorldBuilder, value: str) -> None:
         if m := record_regexp.match(value):
             builder.record_count(parse_integer(m.group("count")))
             builder.record_date(parse_tibia_datetime(m.group("date")))
 
     @classmethod
-    def _parse_creation_date(cls, builder: WorldBuilder, value: str):
+    def _parse_creation_date(cls, builder: WorldBuilder, value: str) -> None:
         parsed_date = datetime.datetime.strptime(value, "%B %Y")
         year, month = parsed_date.year, parsed_date.month
         builder.creation_date(f"{year:d}-{month:02d}")
 
     @classmethod
-    def _parse_battleye_status(cls, builder: WorldBuilder, battleye_string: str):
+    def _parse_battleye_status(cls, builder: WorldBuilder, battleye_string: str) -> None:
         """Parse the BattlEye string and applies the results.
 
         Parameters
         ----------
         builder: :class:`WorldBuilder`
             The builder instance used to set the values.
         battleye_string: :class:`str`
@@ -214,27 +214,27 @@
             additional_info = cols[5].text.strip()
             cls._parse_additional_info(builder, additional_info)
             worlds.append(builder.build())
 
         return worlds
 
     @classmethod
-    def _parse_additional_info(cls, builder: WorldEntryBuilder, additional_info: str):
+    def _parse_additional_info(cls, builder: WorldEntryBuilder, additional_info: str) -> None:
         if "blocked" in additional_info:
             builder.transfer_type(TransferType.BLOCKED)
         elif "locked" in additional_info:
             builder.transfer_type(TransferType.LOCKED)
         else:
             builder.transfer_type(TransferType.REGULAR)
 
         builder.is_experimental("experimental" in additional_info)
         builder.is_premium_only("premium" in additional_info)
 
     @classmethod
-    def _parse_worlds_tables(cls, tables: List[bs4.Tag]):
+    def _parse_worlds_tables(cls, tables: List[bs4.Tag]) -> List[WorldEntry]:
         """Parse the tables and adds the results to the world list.
 
         Parameters
         ----------
         tables: :class:`map` of :class:`bs4.Tag`
             A mapping containing the tables with worlds.
         """
```

### Comparing `tibia.py-6.1.0/tibiapy/urls.py` & `tibia.py-6.2.0/tibiapy/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,25 @@
     -------
     :class:`str`
         The URL to the house's page in Tibia.com.
     """
     return get_tibia_url("community", "houses", page="view", houseid=house_id, world=world)
 
 
+def get_fansites_url() -> str:
+    """Get the Tibia.com URL for the fansites section.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the fansites section.
+    """
+    return get_tibia_url("community", "fansites")
+
+
 def get_world_overview_url() -> str:
     """Get the URL to world overview section in Tibia.com.
 
     Returns
     -------
     :class:`str`
         The URL to the world overview section in Tibia.com.
```

### Comparing `tibia.py-6.1.0/tibiapy/utils.py` & `tibia.py-6.2.0/tibiapy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
         text_tag = table_container.select_one("div.Text")
         if table := table_container.select_one("table.TableContent"):
             tables[text_tag.text.strip()] = table
 
     return tables
 
 
-def try_enum(cls: Type[T], val: Any, default: D = None) -> Union[T, D]:  # noqa: ANN401
+def try_enum(cls: Type[T], val: Any, default: D = None) -> Union[T, D]:
     """Attempt to convert a value into their enum value.
 
     Parameters
     ----------
     cls: :class:`Enum`
         The enum to convert to.
     val:
```

