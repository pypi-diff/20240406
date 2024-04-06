# Comparing `tmp/MarketTime-1.1.2.tar.gz` & `tmp/MarketTime-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarketTime-1.1.2.tar", last modified: Fri Apr  5 08:18:20 2024, max compression
+gzip compressed data, was "MarketTime-1.1.3.tar", last modified: Sat Apr  6 12:16:19 2024, max compression
```

## Comparing `MarketTime-1.1.2.tar` & `MarketTime-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:18:20.877856 MarketTime-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 08:18:13.000000 MarketTime-1.1.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:18:20.877856 MarketTime-1.1.2/MarketTime/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 08:18:13.000000 MarketTime-1.1.2/MarketTime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-05 08:18:13.000000 MarketTime-1.1.2/MarketTime/future_market_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-05 08:18:13.000000 MarketTime-1.1.2/MarketTime/market_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-05 08:18:13.000000 MarketTime-1.1.2/MarketTime/stock_market_time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:18:20.877856 MarketTime-1.1.2/MarketTime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-05 08:18:20.000000 MarketTime-1.1.2/MarketTime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-05 08:18:20.000000 MarketTime-1.1.2/MarketTime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:18:20.000000 MarketTime-1.1.2/MarketTime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 08:18:20.000000 MarketTime-1.1.2/MarketTime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 08:18:20.000000 MarketTime-1.1.2/MarketTime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-05 08:18:20.877856 MarketTime-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-05 08:18:13.000000 MarketTime-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:18:20.877856 MarketTime-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-05 08:18:13.000000 MarketTime-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:16:19.121093 MarketTime-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 12:16:11.000000 MarketTime-1.1.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:16:19.121093 MarketTime-1.1.3/MarketTime/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-06 12:16:11.000000 MarketTime-1.1.3/MarketTime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-06 12:16:11.000000 MarketTime-1.1.3/MarketTime/future_market_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-06 12:16:11.000000 MarketTime-1.1.3/MarketTime/market_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-06 12:16:11.000000 MarketTime-1.1.3/MarketTime/stock_market_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:16:19.121093 MarketTime-1.1.3/MarketTime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-06 12:16:19.000000 MarketTime-1.1.3/MarketTime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-06 12:16:19.000000 MarketTime-1.1.3/MarketTime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 12:16:19.000000 MarketTime-1.1.3/MarketTime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 12:16:19.000000 MarketTime-1.1.3/MarketTime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 12:16:19.000000 MarketTime-1.1.3/MarketTime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-06 12:16:19.121093 MarketTime-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-06 12:16:11.000000 MarketTime-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 12:16:19.121093 MarketTime-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-06 12:16:11.000000 MarketTime-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:16:19.121093 MarketTime-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    38647 2024-04-06 12:16:11.000000 MarketTime-1.1.3/tests/test_future_market_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-06 12:16:11.000000 MarketTime-1.1.3/tests/test_market_time.py
```

### Comparing `MarketTime-1.1.2/LICENSE` & `MarketTime-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MarketTime-1.1.2/MarketTime/future_market_time.py` & `MarketTime-1.1.3/MarketTime/future_market_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,38 +137,41 @@
             30 if FutureMarketTime.in_settlement_day(time) else 45
         )
         night_close = time.replace(hour=5, minute=0, second=0, microsecond=0)
         morning_close = time.replace(
             hour=13, minute=morning_close_minute, second=0, microsecond=0
         )
         today_is_open_day = FutureMarketTime.in_open_day(time)
-        if today_is_open_day and time < morning_close:
-            if time < night_close:
+        if today_is_open_day and time <= morning_close:
+            if time <= night_close:
                 next_close_time = night_close
             else:
                 next_close_time = morning_close
         else:
-            next_close_time = night_close
-            while not FutureMarketTime.in_open_time(next_close_time):
-                next_close_time += timedelta(days=1)
+            if time <= night_close:
+                next_close_time = night_close
+            else:
+                next_close_time = night_close + timedelta(days=1)
+                while not FutureMarketTime.in_open_time(next_close_time):
+                    next_close_time += timedelta(days=1)
         return next_close_time + timedelta(microseconds=1)
 
     @staticmethod
     def last_close_time(time: datetime = None) -> datetime:
         """Return the last close time based on 'time.
         If 'time' is in close time, return 'time'"""
         """8:45 15:00"""
         time = time or datetime.now()
         if not FutureMarketTime.in_open_time(time):
             return time
         morning_open = time.replace(hour=8, minute=45, second=0, microsecond=0)
         night_open = time.replace(hour=15, minute=0, second=0, microsecond=0)
         today_is_open_day = FutureMarketTime.in_open_day(time)
         if today_is_open_day and time >= morning_open:
-            if time > night_open:
+            if time >= night_open:
                 last_close_time = night_open
             else:
                 last_close_time = morning_open
         else:
             last_close_time = night_open - timedelta(days=1)
             while not FutureMarketTime.in_open_time(last_close_time):
                 last_close_time -= timedelta(days=1)
```

### Comparing `MarketTime-1.1.2/MarketTime/market_time.py` & `MarketTime-1.1.3/MarketTime/market_time.py`

 * *Files identical despite different names*

### Comparing `MarketTime-1.1.2/MarketTime/stock_market_time.py` & `MarketTime-1.1.3/MarketTime/stock_market_time.py`

 * *Files identical despite different names*

### Comparing `MarketTime-1.1.2/MarketTime.egg-info/PKG-INFO` & `MarketTime-1.1.3/MarketTime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarketTime
-Version: 1.1.2
+Version: 1.1.3
 Summary: This is a tool to check the time in the market
 Home-page: https://github.com/Liaou3/MarketTime
 Download-URL: 
 Author: VincentLiao
 Author-email: vincent932693@gmail.com
 License: GPLv3
 Requires-Python: >=3.10
```

### Comparing `MarketTime-1.1.2/PKG-INFO` & `MarketTime-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarketTime
-Version: 1.1.2
+Version: 1.1.3
 Summary: This is a tool to check the time in the market
 Home-page: https://github.com/Liaou3/MarketTime
 Download-URL: 
 Author: VincentLiao
 Author-email: vincent932693@gmail.com
 License: GPLv3
 Requires-Python: >=3.10
```

### Comparing `MarketTime-1.1.2/README.md` & `MarketTime-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `MarketTime-1.1.2/setup.py` & `MarketTime-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 PACKAGE_NAME = "MarketTime"
 AUTHOR = "VincentLiao"
 AUTHOR_EMAIL = "vincent932693@gmail.com"
 URL = "https://github.com/Liaou3/MarketTime"
 DOWNLOAD_URL = ""
 
 LICENSE = "GPLv3"
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 DESCRIPTION = "This is a tool to check the time in the market"
 LONG_DESCRIPTION = (HERE/"README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
 INSTALL_REQUIRES = ["datetime"]
 EXTRAS_REQUIRE = {}
 CLASSIFIERS = []
 PYTHON_REQUIRES = ">=3.10"
```

