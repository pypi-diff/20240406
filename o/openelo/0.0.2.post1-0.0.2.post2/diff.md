# Comparing `tmp/openelo-0.0.2.post1.tar.gz` & `tmp/openelo-0.0.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openelo-0.0.2.post1.tar", last modified: Mon Mar 11 10:28:47 2024, max compression
+gzip compressed data, was "openelo-0.0.2.post2.tar", last modified: Fri Apr  5 22:25:46 2024, max compression
```

## Comparing `openelo-0.0.2.post1.tar` & `openelo-0.0.2.post2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 10:28:47.541141 openelo-0.0.2.post1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-11 10:28:47.541141 openelo-0.0.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 10:28:47.541141 openelo-0.0.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 10:28:47.537141 openelo-0.0.2.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 10:28:47.537141 openelo-0.0.2.post1/src/openelo/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 10:28:47.541141 openelo-0.0.2.post1/src/openelo/common/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    11098 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/numericals.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/rating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/team_rating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/common/term.py
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/skill_adjuster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 10:28:47.541141 openelo-0.0.2.post1/src/openelo/systems/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/bradley_terry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/codeforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/elo.py
--rw-r--r--   0 runner    (1001) docker     (127)    21792 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/elommr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/endureelo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/glicko.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/plackett_luce.py
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/thurstone_mosteller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/topcoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/systems/trueskill.py
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-03-11 10:28:39.000000 openelo-0.0.2.post1/src/openelo/team_balancer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 10:28:47.541141 openelo-0.0.2.post1/src/openelo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-11 10:28:47.000000 openelo-0.0.2.post1/src/openelo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-11 10:28:47.000000 openelo-0.0.2.post1/src/openelo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 10:28:47.000000 openelo-0.0.2.post1/src/openelo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-11 10:28:47.000000 openelo-0.0.2.post1/src/openelo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 10:28:47.000000 openelo-0.0.2.post1/src/openelo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:25:46.845752 openelo-0.0.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 22:25:46.845752 openelo-0.0.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12388 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 22:25:46.845752 openelo-0.0.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:25:46.841752 openelo-0.0.2.post2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:25:46.841752 openelo-0.0.2.post2/src/openelo/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:25:46.845752 openelo-0.0.2.post2/src/openelo/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11133 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/numericals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/rating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/team_rating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/common/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/skill_adjuster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:25:46.845752 openelo-0.0.2.post2/src/openelo/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/bradley_terry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/codeforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/elo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22094 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/elommr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/endureelo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/glicko.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/plackett_luce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/thurstone_mosteller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/topcoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/systems/trueskill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-05 22:25:36.000000 openelo-0.0.2.post2/src/openelo/team_balancer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:25:46.845752 openelo-0.0.2.post2/src/openelo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 22:25:46.000000 openelo-0.0.2.post2/src/openelo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-05 22:25:46.000000 openelo-0.0.2.post2/src/openelo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 22:25:46.000000 openelo-0.0.2.post2/src/openelo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 22:25:46.000000 openelo-0.0.2.post2/src/openelo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 22:25:46.000000 openelo-0.0.2.post2/src/openelo.egg-info/top_level.txt
```

### Comparing `openelo-0.0.2.post1/LICENSE` & `openelo-0.0.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/PKG-INFO` & `openelo-0.0.2.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openelo
-Version: 0.0.2.post1
+Version: 0.0.2.post2
 Summary: A set of elo systems written in Python.
 Home-page: https://github.com/BeniaminC/Open-ELO
 Author: Beniamin Condrea
 Author-email: benjamin.condrea@gmail.com
 Keywords: elo,rating system,mmr,competition
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openelo-0.0.2.post1/setup.py` & `openelo-0.0.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='openelo',
-    version='0.0.2-1',
+    version='0.0.2-2',
     author='Beniamin Condrea',
     author_email='benjamin.condrea@gmail.com',
     url='https://github.com/BeniaminC/Open-ELO',
     description='A set of elo systems written in Python.',
     long_description='file: README.md',
     keywords=['elo', 'rating system', 'mmr', 'competition'],
     packages=find_packages(where='src'),
```

### Comparing `openelo-0.0.2.post1/src/openelo/common/aggregation.py` & `openelo-0.0.2.post2/src/openelo/common/aggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from abc import ABC, abstractmethod
 from typing import Any
 
 from .player import Player
 from .term import Rating
 
 
-__all__ = ['TeamSumAggregation', 
-           'TeamAverageAggregation', 
-           'TeamMaxAggregation', 
-           'TeamMinAggregation', 
-           'TeamAverageAggregationN', 
+__all__ = ['TeamSumAggregation',
+           'TeamAverageAggregation',
+           'TeamMaxAggregation',
+           'TeamMinAggregation',
+           'TeamAverageAggregationN',
            'TeamSumAggregationN']
 
 
 class TeamRatingAggregation(ABC):
     '''
     Abstract base class for team rating aggregation.
     '''
@@ -103,15 +103,15 @@
         to be less than or equal to the number of players in each team. Either
         set `best` to either be the best `n` players or the worst `n` players by
         rating.
 
         Args:
             n (:obj:`int`): The number of players per team to aggregate.
 
-            best (:obj:`bool`): Compute the best players (default `True`).
+            best (:obj:`bool`): Compute the best `n` players (default `True`).
 
         Returns:
             :obj:`None`
         '''
         self.n = n
         self.best = best
```

### Comparing `openelo-0.0.2.post1/src/openelo/common/bucket.py` & `openelo-0.0.2.post2/src/openelo/common/bucket.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,11 +46,12 @@
             a (:obj:`float`): First input number.
 
             b (:obj:`float`): Second input number.
 
             width (:obj:`float`): Width of the bucket.
 
         Returns:
-            :obj:`Ordering`
+            :obj:`Ordering`: Return an ordering according to
+            `a` and `b`.
 
     '''
     return Ordering.cmp(bucket(a, width), bucket(b, width))
```

### Comparing `openelo-0.0.2.post1/src/openelo/common/common.py` & `openelo-0.0.2.post2/src/openelo/common/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from dataclasses import dataclass, field
 from typing import Any, Callable, Literal, Optional
 
 from .player import Player
 from .term import TanhTerm
 
 
-__all__ = ['convert_placement_to_standings', 
-           'ContestRatingParams']
+__all__ = ['convert_placement_to_standings',
+           'ContestRatingParams',
+           'EloMMRVariant']
 
 
 Standings = list[tuple[Player, int, int]]
 
 
 def convert_placement_to_standings(placements: list[tuple[Player, int]]) -> Standings:
     '''
@@ -157,15 +158,15 @@
     Given a list of rankings and a rank with a key, return a sub array of rankings
     of the left partial (highest rank of a set of team that is lower than rank). 
     This means teams that are tied in this partial will be included in this set.
 
     Args:
         rankings (:obj:`list[Any]`): List of rankings.
 
-        rank (:obj:`int`) Rank to find the partial.
+        rank (:obj:`int`): Rank to find the partial.
 
         key (:obj:`Callable[..., int]`): function to compare the rankings and rank.
 
     Returns:
         :obj:`list[Any]`: Sub array of ranking of the left partial.
     '''
     if not rankings:
@@ -185,15 +186,15 @@
     Given a list of fankings and a rank with a key, reutrn a sub array of rankings
     of the right partial (lowest rank of a set of team that is higher than rank).
     This means teams that are tied in this partial will be included in the set.
 
     Args:
         rankings (:obj:`list[Any]`): List of rankings.
 
-        rank (:obj:`int`) Rank to find the partial.
+        rank (:obj:`int`): Rank to find the partial.
 
         key (:obj:`Callable[..., int]`): function to compare the rankings and rank.
 
     Returns:
         :obj:`list[Any]`: Sub array of ranking of the right partial.
     '''
     if not rankings:
@@ -213,15 +214,15 @@
     Given a list of rankings and a rank with a key, return a sub array of rankings
     of the left and right partial (lowest/highest of higher/lower ranks, respectively).
     This means teams that are tied in this partial will be included in the set.
 
     Args:
         rankings (:obj:`list[Any]`): List of rankings.
 
-        rank (:obj:`int`) Rank to find the partial.
+        rank (:obj:`int`): Rank to find the partial.
 
         key (:obj:`Callable[..., int]`): function to compare the rankings and rank.
 
     Returns:
         :obj:`list[Any]`: Sub array of ranking of the left and right partials.
     '''
     return find_left_partial(rankings, rank, key) + find_right_partial(rankings, rank, key)
@@ -231,15 +232,15 @@
     '''
     Given a list of rankings and a rank with a key, return a sub array of rankings
     of the ranking that are less than rank.
 
     Args:
         rankings (:obj:`list[Any]`): List of rankings.
 
-        rank (:obj:`int`) Rank to find sub array less than this value.
+        rank (:obj:`int`): Rank to find sub array less than this value.
 
         key (:obj:`Callable[..., int]`): function to compare the rankings and rank.
 
     Returns:
         :obj:`list[Any]`: Sub array of ranking less than rank.
     '''
     left_i = bisect_left(rankings, rank, key=key)
@@ -252,15 +253,15 @@
     '''
     Given a list of rankings and a rank with a key, return a sub array of rankings
     of the ranking that are less than or equal to rank.
 
     Args:
         rankings (:obj:`list[Any]`): List of rankings.
 
-        rank (:obj:`int`) Rank to find sub array less than or equal to this value.
+        rank (:obj:`int`): Rank to find sub array less than or equal to this value.
 
         key (:obj:`Callable[..., int]`): function to compare the rankings and rank.
 
     Returns:
         :obj:`list[Any]`: Sub array of ranking less than or equal to rank.
     '''
     right_i = bisect_right(rankings, rank, key=key)
@@ -273,15 +274,15 @@
     '''
     Given a list of rankings and a rank with a key, return a sub array of rankings
     of the ranking that are greater than rank.
 
     Args:
         rankings (:obj:`list[Any]`): List of rankings.
 
-        rank (:obj:`int`) Rank to find sub array greater than this value.
+        rank (:obj:`int`): Rank to find sub array greater than this value.
 
         key (:obj:`Callable[..., int]`): function to compare the rankings and rank.
 
     Returns:
         :obj:`list[Any]`: Sub array of ranking greater than rank.
     '''
     right_i = bisect_right(rankings, rank, key=key)
@@ -294,15 +295,15 @@
     '''
     Given a list of rankings and a rank with a key, return a sub array of rankings
     of the ranking that are greater than or equal to rank.
 
     Args:
         rankings (:obj:`list[Any]`): List of rankings.
 
-        rank (:obj:`int`) Rank to find sub array greater than or equal to this value.
+        rank (:obj:`int`): Rank to find sub array greater than or equal to this value.
 
         key (:obj:`Callable[..., int]`): function to compare the rankings and rank.
 
     Returns:
         :obj:`list[Any]`: Sub array of ranking greater than or eqaul to rank.
     '''
     left_i = bisect_left(rankings, rank, key=key)
@@ -315,15 +316,15 @@
     '''
     Given a list of rankings and a rank with a key, return a sub array of rankings
     of the ranking that are less than rank.
 
     Args:
         rankings (:obj:`list[Any]`): List of rankings.
 
-        rank (:obj:`int`) Rank to find sub array less than this value.
+        rank (:obj:`int`): Rank to find sub array less than this value.
 
         key (:obj:`Callable[..., int]`): function to compare the rankings and rank.
 
     Returns:
         :obj:`list[Any]`: Sub array of ranking equal to rank.
     '''
     left_i = bisect_left(rankings, rank, key=key)
```

### Comparing `openelo-0.0.2.post1/src/openelo/common/constants.py` & `openelo-0.0.2.post2/src/openelo/common/constants.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/common/numericals.py` & `openelo-0.0.2.post2/src/openelo/common/numericals.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/common/player.py` & `openelo-0.0.2.post2/src/openelo/common/player.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import deque
 from dataclasses import dataclass, field
 from typing import Optional, Self
 from .constants import DEFAULT_MU, DEFAULT_SIG, DEFAULT_SIG_LIMIT
 from .term import Rating, TanhTerm, robust_average
 
 
-__all__ = ['Player', 
+__all__ = ['Player',
            'PlayersByName']
 
 
 @dataclass
 class PlayerEvent:
     contest_index: Optional[int]
     rating_mu: float
@@ -79,15 +79,15 @@
 
     def times_played_excl(self) -> int:
         '''
         Return the `length - 1` of the player's played history. This is to get the number of games
         played if a history event has already been appended.
 
         Returns:
-            :obj:`int`: 
+            :obj:`int`: The number of games excluding the unrecorded initialized game.
         '''
         return len(self.event_history) - 1
 
     def is_newcomer(self) -> bool:
         '''
         Returns a boolean of if a player has zero games or not.
 
@@ -185,30 +185,30 @@
 
     def add_noise_and_collapse(self, sig_noise: float) -> None:
         '''
         Adds noise to the approximate posterior and set the normal factor to the approximate posterior.
         Clears all the logistic factors.
 
         Args:
-            sig_noise :obj:`float`: the noise added to the approximate posterior.
+            sig_noise (:obj:`float`): the noise added to the approximate posterior.
         
         Return::
             :obj:`None`
         
         '''
         self.approx_posterior = self.approx_posterior.with_noise(sig_noise)
         self.normal_factor = self.approx_posterior
         self.logistic_factors.clear()
 
     def add_noise_in_front(self, sig_noise: float) -> None:
         '''
         Adds noise to the normal factor from the logstic factors.
 
         Args:
-            sig_noise :obj:`float`: the noise added to the approximate posterior and changes the weight
+            sig_noise (:obj:`float`): the noise added to the approximate posterior and changes the weight
             of each logistic factor.
 
         Returns:
             :obj:`None`
         '''
         decay = 1.0
         decay *= sig_noise / self.approx_posterior.sig
@@ -219,18 +219,18 @@
 
     def add_noise_best(self, sig_noise: float, transfer_speed: float) -> None:
         '''
         Adds noise to the approximate posterior and transfers weights from the logistic
         factors to the normal (Gaussian) factors.
 
         Args:
-            sig_noise :obj:`float`: the noise added to the approximate posterior and changes the weight
+            sig_noise (:obj:`float`): the noise added to the approximate posterior and changes the weight
             of each logistic factor.
 
-            transfer_speed :obj:`float`: Transfer speed of weights from the logistic factors to the normal
+            transfer_speed (:obj:`float`): Transfer speed of weights from the logistic factors to the normal
             (Gassian) factor.
         
         Returns:
             :obj:`None`
         '''
         # sig noise is beta, transfer speed is rho
         new_posterior = self.approx_posterior.with_noise(sig_noise)  # u_i, sqrt(sig, beta)
@@ -247,17 +247,17 @@
             r.w_out *= transfer * decay
 
     def init_player_event(self, lo: int, contest_time: int = 0) -> None:
         '''
         Initializes a player event with the `lo` placement and the contest time.  The values initialized are placeholders (zeroes).
 
         Args:
-            lo :obj:`int`: The placement of the player.
+            lo (:obj:`int`): The placement of the player.
 
-            contest_time :obj:`int`: The contest time of the event.
+            contest_time (:obj:`int`): The contest time of the event.
         
         Returns:
             :obj:`None`
         '''
         self.delta_time = contest_time - self.update_time
         self.update_time = contest_time
         self.event_history.append(
```

### Comparing `openelo-0.0.2.post1/src/openelo/common/rating_system.py` & `openelo-0.0.2.post2/src/openelo/common/rating_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         '''
         Abstract method required to be defined for `RatingSystem`.
 
         Args:
             params (:obj:`ContestRatingParams`): Contest rating parameters for individual
             contest.
 
-            standings(:obj:`Standings`): List of `Player` objects with
+            standings (:obj:`Standings`): List of `Player` objects with
             their standings (start, end).
         '''
         pass
 
     @staticmethod
     def init_players_event(standings: Standings, contest_time: int = 0) -> None:
         '''
@@ -30,15 +30,15 @@
         If the rating system does not utilize contest time `contest_time`, then
         do not set it.
 
         Args:
             standings (:obj:`Standings`): List of `Player` objects with
             their standings (start, end).
 
-            contest_time(:obj:`int`): Contest time (in seconds).
+            contest_time (:obj:`int`): Contest time (in seconds).
         Returns:
             :obj:`None`
         '''
         with concurrent.futures.ThreadPoolExecutor() as executor:
             for player, lo, _ in standings:
                 executor.submit(player.init_player_event, lo, contest_time)
```

### Comparing `openelo-0.0.2.post1/src/openelo/common/statistics.py` & `openelo-0.0.2.post2/src/openelo/common/statistics.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/common/team_rating_system.py` & `openelo-0.0.2.post2/src/openelo/common/team_rating_system.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/common/term.py` & `openelo-0.0.2.post2/src/openelo/common/term.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,37 +16,37 @@
     '''
     @abstractmethod
     def eval(self, x: float, order: Ordering, split_ties: bool) -> tuple[float, float]:
         '''
         Abstract method to be defined.
 
         Args:
-            x :obj:`float`: Scalar value for scalar minimization.
+            x (:obj:`float`): Scalar value for scalar minimization.
 
-            order :obj:`Ordering`: Relative ordering.
+            order (:obj:`Ordering`): Relative ordering.
 
-            split_ties :obj:`bool`: Boolean to split ties to evaluate to half a win and half a loss.
+            split_ties (:obj:`bool`): Boolean to split ties to evaluate to half a win and half a loss.
 
         Return:
             :obj:tuple[float, float]: Returns the value and its respective derivative.
         '''
         pass
 
     def evals(self, x: float, ranks: list[int], my_rank: int, split_ties: bool) -> tuple[float, float]:
         '''
         Evaulate a list of ranks according to a scalar value `x` relative to a specific rank `my_rank`.
 
         Args:
-            x :obj:`float`: Scalar value for scalar minimization.
+            x (:obj:`float`): Scalar value for scalar minimization.
 
-            ranks :obj:`list[int]`: A list of ranks.
+            ranks (:obj:`list[int]`): A list of ranks.
 
-            my_rank :obj:`int`: Rank to evalulate the minimization relative to the ranks in the list.
+            my_rank (:obj:`int`): Rank to evalulate the minimization relative to the ranks in the list.
 
-            split_ties :obj:`bool`: Boolean to split ties to evaluate to half a win and half a loss.
+            split_ties (:obj:`bool`): Boolean to split ties to evaluate to half a win and half a loss.
 
         Return:
             :obj:tuple[float, float]: Returns the value and its respective derivative.
         '''
         if len(ranks) == 1:
             return self.eval(x, Ordering.cmp(ranks[0], my_rank), split_ties)
         start, end = Term.equal_range(ranks, my_rank)
@@ -70,17 +70,17 @@
 
     @staticmethod
     def equal_range(ranks: list[int], my_rank: int) -> tuple[int, int]:
         '''
         Auxillary method to find the indices of equal rank.
 
         Args:
-             ranks :obj:`list[int]`: A list of ranks.
+             ranks (:obj:`list[int]`): A list of ranks.
 
-             my_rank :obj:`int`: Rank to find equivalent ranks.
+             my_rank (:obj:`int`): Rank to find equivalent ranks.
 
         Returns:
             :obj:`tuplep[int, int]`: Indices range of equal rank.
         '''
         left = bisect_left(ranks, my_rank)
         right = bisect_right(ranks, my_rank, lo=left)
         return left, right
@@ -96,19 +96,19 @@
 
     def eval(self, x: float, order: Ordering, split_ties: bool) -> tuple[float, float]:
         '''
         Method to evaluate the minimization according to the order. This uses normal (Gaussian)
         cdf and pdf to compute value.
 
         Args:
-            x :obj:`float`: Scalar value for scalar minimization.
+            x (:obj:`float`): Scalar value for scalar minimization.
 
-            order :obj:`Ordering`: Relative ordering.
+            order (:obj:`Ordering`): Relative ordering.
 
-            split_ties :obj:`bool`: Boolean to split ties to evaluate to half a win and half a loss.
+            split_ties (:obj:`bool`): Boolean to split ties to evaluate to half a win and half a loss.
 
         Return:
             :obj:tuple[float, float]: Returns the value and its respective derivative.
         '''
         z = (x - self.mu) / self.sig
         pdf = standard_normal_pdf(z) / self.sig
         pdf_prime = -z * pdf / self.sig
@@ -137,30 +137,30 @@
                     return (val, pdf_pp / pdf - val * val)
 
     def with_noise(self, sig_noise: float) -> 'Rating':
         '''
         Compute the new deviation with noise.
 
         Args:
-            sig_noise :obj:`float`: Noise to add to the rating deviation.
+            sig_noise (:obj:`float`): Noise to add to the rating deviation.
 
         Returns:
             :obj:`Rating`: New Rating with added noise.
         '''
         return Rating(self.mu, (self.sig ** 2 + sig_noise ** 2) ** 0.5)
 
     def towards_noise(self, decay: float, limit: Self) -> 'Rating':
         '''
         Compute the new deviation towards the `limit` rating (mu and sig).
         This change is proportional to the `decay`.
 
         Args:
-            decay :obj:`float`: Decay rate to move towards noise.
+            decay (:obj:`float`): Decay rate to move towards noise.
 
-            linit :obj:`Rating`: Rating to move towards.
+            linit (:obj:`Rating`): Rating to move towards.
 
         Returns:
             :obj:`Rating`: New Rating towards the limit.
         '''
         mu_diff = self.mu - limit.mu
         sig_sq_diff = self.sig ** 2 - limit.sig ** 2
         return Rating(limit.mu + mu_diff * decay, (limit.sig ** 2 + sig_sq_diff * decay ** 2) ** 0.5)
@@ -174,19 +174,19 @@
 
     def eval(self, x: float, order: Ordering, split_ties: bool):
         '''
         Method to evaluate the minimization according to the order. This uses logistic
         cdf and pdf to compute value.
 
         Args:
-            x :obj:`float`: Scalar value for scalar minimization.
+            x (:obj:`float`): Scalar value for scalar minimization.
 
-            order :obj:`Ordering`: Relative ordering.
+            order (:obj:`Ordering`): Relative ordering.
 
-            split_ties :obj:`bool`: Boolean to split ties to evaluate to half a win and half a loss.
+            split_ties (:obj:`bool`): Boolean to split ties to evaluate to half a win and half a loss.
 
         Return:
             :obj:tuple[float, float]: Returns the value and its respective derivative.
         '''
         val, val_prime = self.base_values(x)
         match order:
             case Ordering.LESS:
@@ -201,15 +201,15 @@
 
     @classmethod
     def from_rating(cls, rating: Rating) -> Self:
         '''
         Create a new `TanhTerm` from rating.
 
         Args:
-            rating :obj:`Rating`
+            rating (:obj:`Rating`)
 
         Returns:
             :obj:`TanhTerm`
         '''
         w = TANH_MULTIPLIER / rating.sig
         return cls(rating.mu, w * 0.5, w)
 
@@ -223,36 +223,36 @@
         return self.w_arg * self.w_out * 2. / TANH_MULTIPLIER ** 2
 
     def base_values(self, x: float) -> tuple[float, float]:
         '''
         Given a scalar value, return the value and derivative.
 
         Args:
-            x :obj:`float`: Value
+            x (:obj:`float`): Value
         
         Returns:
             :obj:`tuple[float, float]`: Computed value with derivative.
         '''
         z = (x - self.mu) * self.w_arg
         val = -math.tanh(z) * self.w_out
         val_prime = -math.cosh(z) ** -2 * self.w_arg * self.w_out
         return val, val_prime
 
     def evals(self, x: float, ranks: list[int], my_rank: int, split_ties: bool) -> tuple[float, float]:
         '''
         Compute the value and derivative of ranks equal to rank.
 
         Args:
-            x :obj:`float`: Scalar value for scalar minimization.
+            x (:obj:`float`): Scalar value for scalar minimization.
 
-            ranks :obj:`list[int]`: A list of ranks.
+            ranks (:obj:`list[int])`: A list of ranks.
 
-            my_rank :obj:`int`: Rank to evalulate the minimization relative to the ranks in the list.
+            my_rank (:obj:`int`): Rank to evalulate the minimization relative to the ranks in the list.
 
-            split_ties :obj:`bool`: Boolean to split ties to evaluate to half a win and half a loss.
+            split_ties (:obj:`bool`): Boolean to split ties to evaluate to half a win and half a loss.
 
         Return:
             :obj:tuple[float, float]: Returns the value and its respective derivative.
         '''
         if len(ranks) == 1:
             return self.eval(x, Ordering.cmp(ranks[0], my_rank), split_ties)
         val, val_prime = self.base_values(x)
@@ -269,19 +269,19 @@
 
 def robust_average(all_ratings: Iterable[TanhTerm], offset: float, slope: float) -> float:
     '''
     Compute the robust average of `TanhTerm`s, given the offset and slope.  This uses Newton's
     method to solve for a scalar function.
 
     Args:
-        all_ratings :obj:`Iterable[TanhTerm]`: All the tanh terms.
+        all_ratings (:obj:`Iterable[TanhTerm])`: All the tanh terms.
 
-        offset :obj:`float`: The starting offset of the reduction.
+        offset (:obj:`float`): The starting offset of the reduction.
 
-        slope :obj:`float`: The starting slope (or derivative) of the reduction.
+        slope (:obj:`float`): The starting slope (or derivative) of the reduction.
     '''
     if isinstance(all_ratings, (Iterator, Generator)):
         raise TypeError('robust_average must accept an iterable which isn\'t consumed (i.e. a list or tuple).')
     bounds = BOUNDS
 
     def f(x: float) -> tuple[float, float]:
         def inner(term: TanhTerm):
```

### Comparing `openelo-0.0.2.post1/src/openelo/skill_adjuster.py` & `openelo-0.0.2.post2/src/openelo/skill_adjuster.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/systems/__init__.py` & `openelo-0.0.2.post2/src/openelo/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/systems/bradley_terry.py` & `openelo-0.0.2.post2/src/openelo/systems/bradley_terry.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ..common.ordering import Ordering
 from ..common.player import Player
 from ..common.rating_system import RatingSystem
 from ..common.team_rating_system import TeamRating, TeamRatingSystem
 from ..common.term import Rating
 
 
-__all__ = ['BradleyTerry', 
+__all__ = ['BradleyTerry',
            'BradleyTerryPartial']
 
 
 @dataclass
 class BradleyTerry(RatingSystem, TeamRatingSystem):
     '''
     Bradley-Terry Rating System.
```

### Comparing `openelo-0.0.2.post1/src/openelo/systems/codeforce.py` & `openelo-0.0.2.post2/src/openelo/systems/codeforce.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/systems/elo.py` & `openelo-0.0.2.post2/src/openelo/systems/elo.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/systems/elommr.py` & `openelo-0.0.2.post2/src/openelo/systems/elommr.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,14 @@
         def _team_tanh_terms(team_i: TeamRating):
             return TanhTerm.from_rating(Rating(team_i.rating.mu, (agg_sig_perfs[team_i.team] + team_i.rating.sig) ** 0.5))
         with concurrent.futures.ThreadPoolExecutor() as executor:
             team_tanh_terms = list(executor.map(_team_tanh_terms, team_ratings))
         mul = 1. if self.split_ties else 2.
 
         def _update_player_rating(team_i: TeamRating):
-
             team_i_players = team_standings[team_i.team]['players']
             team_size = len(team_i_players)
             bounds = (1500 - (7500 * team_size), 1500 + (7500 * team_size))
             lo = bisect_left(team_ratings, team_i.rank, key=lambda x: x.rank)
             hi = bisect_right(team_ratings, team_i.rank, key=lambda x: x.rank)
 
             def f(x):
@@ -144,21 +143,21 @@
                 itr3 = (eval_grea(term, x) for term in team_tanh_terms[hi:])
                 chained = chain(
                     itr1,
                     itr2,
                     itr3)
                 acc = reduce(lambda x, y: (x[0] + y[0], x[1] + y[1]), chained, (0., 0.))
                 return acc
-            mu_perf = clamp(solve_newton(bounds, f), params.perf_floor, params.perf_ceiling)
+            # TODO: make team performance clamp coincide with aggregation
+            team_mu_perf = clamp(solve_newton(bounds, f), params.perf_floor * team_size, params.perf_ceiling * team_size)
             team_i_mu = team_i.rating.mu
 
             def _update_individual(player: Player):
-
                 teammates_rating = team_i_mu - player.approx_posterior.mu
-                player_mu_perf = mu_perf - teammates_rating
+                player_mu_perf = clamp(team_mu_perf - teammates_rating, params.perf_floor, params.perf_ceiling)
                 weight = self.compute_weight(params.weight, self.weight_limit, self.noob_delay, player.times_played_excl())
                 sig_perf = self.compute_sig_perf(weight, self.sig_limit, self.drift_per_day)
                 player.update_rating_with_logistic(Rating(player_mu_perf, sig_perf), self.history_len)
             with concurrent.futures.ThreadPoolExecutor() as executor:
                 executor.map(_update_individual,  team_i_players)
         with concurrent.futures.ThreadPoolExecutor() as executor:
             executor.map(_update_player_rating, team_ratings)
@@ -397,19 +396,20 @@
 
                 def f(x):
                     res: list[tuple[float, float]] = []
                     for rating, ranks in tanh_subsample:
                         res.append(rating.evals(x, ranks, team_i.rank, self.split_ties))
                     acc = reduce(lambda x, y: (x[0] + y[0], x[1] + y[1]), res, (0., 0.))
                     return acc
-                team_mu_perf = clamp(solve_newton(bounds, f), params.perf_floor, params.perf_ceiling)
+                # TODO: make team performance clamp coincide with aggregation
+                team_mu_perf = clamp(solve_newton(bounds, f), params.perf_floor * team_size, params.perf_ceiling * team_size)
 
             def _update_individual(player: Player):
                 teammates_rating = team_i_mu - player.approx_posterior.mu
-                player_mu_perf = team_mu_perf - teammates_rating
+                player_mu_perf = clamp(team_mu_perf - teammates_rating, params.perf_floor, params.perf_ceiling)
                 weight = self.compute_weight(params.weight, self.weight_limit, self.noob_delay, player.times_played_excl())
                 sig_perf = self.compute_sig_perf(weight, self.sig_limit, self.drift_per_day)
                 if self.variant == EloMMRVariant.gaussian():
                     player.update_rating_with_normal(Rating(player_mu_perf, sig_perf))
                 elif self.variant == EloMMRVariant.logistic():
                     player.update_rating_with_logistic(Rating(player_mu_perf, sig_perf), self.subsample_size)
             with concurrent.futures.ThreadPoolExecutor() as executor:
```

### Comparing `openelo-0.0.2.post1/src/openelo/systems/endureelo.py` & `openelo-0.0.2.post2/src/openelo/systems/endureelo.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/systems/glicko.py` & `openelo-0.0.2.post2/src/openelo/systems/glicko.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 @dataclass
 class Glicko(RatingSystem, TeamRatingSystem):
     '''
     Glicko rating system.
     '''
     beta: float = DEFAULT_BETA
-    scaling: float = 400.
     weight_limit: float = DEFAULT_WEIGHT_LIMIT
     noob_delay: list[float] = field(default_factory=list)
     sig_limit: float = DEFAULT_SIG_LIMIT
     drift_per_day: float = DEFAULT_DRIFTS_PER_DAY
 
     @staticmethod
     def _win_probability(sig_perf: float, player: Rating, foe: Rating) -> float:
@@ -83,32 +82,28 @@
             mu = my_rating.mu + update
             player.update_rating(Rating(mu, sig), 0.)
         with concurrent.futures.ThreadPoolExecutor() as executor:
             for rating, my_lo, _ in standings:
                 executor.submit(_update_player_rating, rating, my_lo)
 
     @staticmethod
-    def _g(sig: float, q: float = GLICKO_Q):
-        return 1. / (((1 + 3 * q ** 2 * sig) / pi ** 2) ** 0.5)
+    def _g(sig_sq: float, sig_perf: float):
+        return 1. / (1 + (sig_sq / sig_perf ** 2)) ** 0.5
 
-    @staticmethod
-    def _pr_i(mu_i: float, mu_j: float, sig_sq_i: float, sig_sq_j: float, q: float, D: float):
-        inner_g = (sig_sq_i + sig_sq_j)
-        diff_mu = (mu_i - mu_j)
-        denom = (1 + 10 ** ((-Glicko._g(inner_g, q) * diff_mu) / D))
-        return 1. / denom
+    # @staticmethod
+    # def _pr_i(mu_i: float, mu_j: float, sig_sq_i: float, sig_sq_j: float, sig_perf: float, scale: float):
+    #     inner_g_sq = (sig_sq_i + sig_sq_j + sig_perf ** 2)
+    #     diff_mu = (mu_i - mu_j)
+    #     denom = (1 + 10 ** ((-Glicko._g(inner_g_sq, sig_perf) * diff_mu) / scale))
+    #     return 1. / denom
 
     @staticmethod
     def _r(N: int, rank_i: int):
         return (N - rank_i) / comb(N, 2)
 
-    @staticmethod
-    def _d_sq_i(pr_i: float, sig_j: float):
-        return (Glicko._g(sig_j) ** 2) * pr_i * (1. - pr_i)
-
     def team_round_update(self,
                           params: ContestRatingParams,
                           standings: Standings,
                           agg: TeamRatingAggregation,
                           contest_time: int = 0) -> None:
         '''
         Update the player ratings in teams according to their team and rank.
@@ -118,60 +113,60 @@
 
             standings (:obj:`Standings`): Standings of each player
             according to their `team` and `rank`. Must be in order.
         '''
         sig_perf = self.beta / ((self.weight_limit * params.weight) ** 0.5)
         gli_q = TANH_MULTIPLIER / sig_perf
         self.init_players_event(standings, contest_time=contest_time)
+
         def _update_player(player: Player):
             weight = self.compute_weight(params.weight, self.weight_limit, self.noob_delay, player.times_played_excl())
             sig_drift = self.compute_sig_drift(weight, self.sig_limit, self.drift_per_day, float(player.delta_time))
             player.add_noise_and_collapse(sig_drift)
         with concurrent.futures.ThreadPoolExecutor() as executor:
-            for player, _, _ in standings:
-                executor.submit(_update_player, player)
+            executor.map(_update_player, (player for player, _, _ in standings))
         team_standings = self.convert_to_teams(standings)
         team_ratings = list(TeamRating(team, team_info['rank'], agg(team_info['players'])) for team, team_info in team_standings.items())
         team_ratings.sort(key=lambda team: team.rank)
         N = len(team_ratings)
         prob_denom = comb(N, 2)
 
         def _update_player_rating(relative_rank: int, team_i: TeamRating):
             team_i_mu = team_i.rating.mu
             team_i_sig_sq = team_i.rating.sig
             pr_i = 0.
-            delta = 0.
-            mu_summation = 0.
-            num_players_in_team = len(team_standings[team_i.team])
+            info = 0.
+            update = 0.
+            team_i_players = team_standings[team_i.team]['players']
+            num_players_in_team = len(team_i_players)
             r_i = (N - relative_rank) / prob_denom
             for team_j in team_ratings:
                 if team_i is team_j:
                     continue
-                team_j_mu = team_j.rating.mu
                 team_j_sig_sq = team_j.rating.sig
-                pr_i += Glicko._pr_i(team_i_mu, team_j_mu, team_i_sig_sq, team_j_sig_sq, gli_q, self.scaling)
+                pr_i += Glicko._win_probability(sig_perf, team_i.rating, team_j.rating)  # TODO: make parameter for scale factor
             pr_i /= prob_denom
             for team_j in team_ratings:
                 if team_i is team_j:
                     continue
-                team_j_sig = team_j.rating.sig
-                mu_summation += Glicko._g(team_j_sig) * (r_i - pr_i)
-            for team_j in team_ratings:
-                if team_i is team_j:
-                    continue
-                team_j_sig = team_j.rating.sig
-                delta += Glicko._g(team_j_sig) ** 2 * pr_i * (1 - pr_i)
-            d_sqr_i = 1. / ((gli_q ** 2) * delta)
-            team_new_mu = team_i_mu + (gli_q / ((1. / team_i_sig_sq) + (1. / d_sqr_i))) * mu_summation
-            team_new_sig_sq = (1. / ((1. / team_i_sig_sq) + (1. / d_sqr_i)))
+                team_j_sig_sq = team_j.rating.sig
+                g = Glicko._g(team_j_sig_sq, sig_perf)
+                info += g * g * pr_i * (1 - pr_i)
+                update += g * (r_i - pr_i)
+            info *= gli_q * gli_q
+            team_new_sig_sq = 1. / ((1. / team_i_sig_sq) + info)
+            update *= gli_q * team_new_sig_sq
             team_new_sig = team_new_sig_sq ** 0.5
-            for player in team_standings[team_i.team]['players']:
+            team_new_mu = team_i_mu + update
+
+            def _update_individual(player: Player):
                 old_mu = player.approx_posterior.mu
                 old_sig = player.approx_posterior.sig
-                w_mu = (1. / num_players_in_team)
-                w_sig = (1. / num_players_in_team)
+                w_mu = 1. / num_players_in_team
+                w_sig = 1. / num_players_in_team
                 new_mu = old_mu + w_mu * (team_new_mu - team_i_mu)
                 new_sig = max(1e-4, old_sig + w_sig * (team_new_sig - team_i_sig_sq ** 0.5))
                 player.update_rating(Rating(new_mu, new_sig), 0)
-
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                executor.map(_update_individual,  team_i_players)
         with concurrent.futures.ThreadPoolExecutor() as executor:
             executor.map(_update_player_rating, *zip(*((i+1, team_i) for i, team_i in enumerate(team_ratings))))
```

### Comparing `openelo-0.0.2.post1/src/openelo/systems/plackett_luce.py` & `openelo-0.0.2.post2/src/openelo/systems/plackett_luce.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/systems/thurstone_mosteller.py` & `openelo-0.0.2.post2/src/openelo/systems/thurstone_mosteller.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/systems/topcoder.py` & `openelo-0.0.2.post2/src/openelo/systems/topcoder.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/systems/trueskill.py` & `openelo-0.0.2.post2/src/openelo/systems/trueskill.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo/team_balancer.py` & `openelo-0.0.2.post2/src/openelo/team_balancer.py`

 * *Files identical despite different names*

### Comparing `openelo-0.0.2.post1/src/openelo.egg-info/PKG-INFO` & `openelo-0.0.2.post2/src/openelo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openelo
-Version: 0.0.2.post1
+Version: 0.0.2.post2
 Summary: A set of elo systems written in Python.
 Home-page: https://github.com/BeniaminC/Open-ELO
 Author: Beniamin Condrea
 Author-email: benjamin.condrea@gmail.com
 Keywords: elo,rating system,mmr,competition
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openelo-0.0.2.post1/src/openelo.egg-info/SOURCES.txt` & `openelo-0.0.2.post2/src/openelo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

