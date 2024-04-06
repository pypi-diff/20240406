# Comparing `tmp/football_stats_scraper-0.1.1-py3-none-any.whl.zip` & `tmp/football_stats_scraper-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4417 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      112 b- defN 24-Apr-06 18:43 src/__init__.py
+Zip file size: 4391 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       70 b- defN 24-Apr-06 20:57 src/__init__.py
 -rw-rw-r--  2.0 unx      339 b- defN 24-Apr-06 19:59 src/defines.py
 -rw-rw-r--  2.0 unx      421 b- defN 24-Apr-06 19:26 src/enums.py
 -rw-rw-r--  2.0 unx     3587 b- defN 24-Apr-06 20:24 src/football-cli.py
--rw-rw-r--  2.0 unx     1416 b- defN 24-Apr-06 20:54 football_stats_scraper-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-06 20:54 football_stats_scraper-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       65 b- defN 24-Apr-06 20:54 football_stats_scraper-0.1.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        4 b- defN 24-Apr-06 20:54 football_stats_scraper-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      752 b- defN 24-Apr-06 20:54 football_stats_scraper-0.1.1.dist-info/RECORD
-9 files, 6788 bytes uncompressed, 3105 bytes compressed:  54.3%
+-rw-rw-r--  2.0 unx     1416 b- defN 24-Apr-06 20:58 football_stats_scraper-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-06 20:58 football_stats_scraper-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       65 b- defN 24-Apr-06 20:58 football_stats_scraper-0.1.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        4 b- defN 24-Apr-06 20:58 football_stats_scraper-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      751 b- defN 24-Apr-06 20:58 football_stats_scraper-0.1.2.dist-info/RECORD
+9 files, 6745 bytes uncompressed, 3079 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: src/enums.py
 Comment: 
 
 Filename: src/football-cli.py
 Comment: 
 
-Filename: football_stats_scraper-0.1.1.dist-info/METADATA
+Filename: football_stats_scraper-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: football_stats_scraper-0.1.1.dist-info/WHEEL
+Filename: football_stats_scraper-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: football_stats_scraper-0.1.1.dist-info/entry_points.txt
+Filename: football_stats_scraper-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: football_stats_scraper-0.1.1.dist-info/top_level.txt
+Filename: football_stats_scraper-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: football_stats_scraper-0.1.1.dist-info/RECORD
+Filename: football_stats_scraper-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/__init__.py

```diff
@@ -1,2 +1 @@
-from .enums import Leagues, ReturnFormats
 from .defines import interesting_league_table_columns, table_base_url
```

## Comparing `football_stats_scraper-0.1.1.dist-info/METADATA` & `football_stats_scraper-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: football-stats-scraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python script to scrape football league tables and fixtures
 Home-page: https://github.com/yourusername/football-stats-scraper
 Author: John Murtagh
 Author-email: john90murtagh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `football_stats_scraper-0.1.1.dist-info/RECORD` & `football_stats_scraper-0.1.2.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-src/__init__.py,sha256=fKjfWPhyCHAk4C-Bpu9y72_dJ0Ipdpup-Jx6CJE8HZw,112
+src/__init__.py,sha256=nqUOaENVsygYiy9H0b98CPY-m4-iAVTXVGvv5mATDDM,70
 src/defines.py,sha256=sbVJ6COs2QvDlmbp9MZd_8SyDrMVFL6Q9vVwCMvibpE,339
 src/enums.py,sha256=IDC5n-ufy5cYNQ7eW_q3DN0iYTmgJRFLCx6GytBsKo8,421
 src/football-cli.py,sha256=m6DW4PKlf4NIJZFZW1yCCaQUpB3qPvM__aHgsIJjMRQ,3587
-football_stats_scraper-0.1.1.dist-info/METADATA,sha256=zbKZv-p3q_8KoKKx-q2Jj9rI3FB4NcWCVD-cKcMJikM,1416
-football_stats_scraper-0.1.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-football_stats_scraper-0.1.1.dist-info/entry_points.txt,sha256=mZBTkMIseUfCEFsoXcjVzNi9V4k4tHW_PvovSOkydkQ,65
-football_stats_scraper-0.1.1.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
-football_stats_scraper-0.1.1.dist-info/RECORD,,
+football_stats_scraper-0.1.2.dist-info/METADATA,sha256=Yn3_bsfA8IARtYxBria74oSyXby1WBvwF2ichDNTmrw,1416
+football_stats_scraper-0.1.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+football_stats_scraper-0.1.2.dist-info/entry_points.txt,sha256=mZBTkMIseUfCEFsoXcjVzNi9V4k4tHW_PvovSOkydkQ,65
+football_stats_scraper-0.1.2.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
+football_stats_scraper-0.1.2.dist-info/RECORD,,
```

