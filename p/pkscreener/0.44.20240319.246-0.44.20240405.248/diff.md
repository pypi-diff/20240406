# Comparing `tmp/pkscreener-0.44.20240319.246.tar.gz` & `tmp/pkscreener-0.44.20240405.248.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240319.246.tar", last modified: Tue Mar 19 06:44:54 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240405.248.tar", last modified: Fri Apr  5 23:49:04 2024, max compression
```

## Comparing `pkscreener-0.44.20240319.246.tar` & `pkscreener-0.44.20240405.248.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 06:44:54.739933 pkscreener-0.44.20240319.246/
--rw-rw-rw-   0        0        0     1086 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-03-19 06:44:54.739933 pkscreener-0.44.20240319.246/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 06:44:54.724303 pkscreener-0.44.20240319.246/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 06:44:54.739933 pkscreener-0.44.20240319.246/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     8480 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2571 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27427 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    15888 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     7653 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    16886 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48873 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   106798 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    43484 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    77220 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-03-19 06:44:42.000000 pkscreener-0.44.20240319.246/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   108017 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    16371 2024-03-19 06:40:39.000000 pkscreener-0.44.20240319.246/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-03-19 06:44:54.739933 pkscreener-0.44.20240319.246/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-03-19 06:44:54.000000 pkscreener-0.44.20240319.246/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-03-19 06:44:54.000000 pkscreener-0.44.20240319.246/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 06:44:54.000000 pkscreener-0.44.20240319.246/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-03-19 06:44:54.000000 pkscreener-0.44.20240319.246/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-19 06:44:54.000000 pkscreener-0.44.20240319.246/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-03-19 06:44:54.000000 pkscreener-0.44.20240319.246/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-19 06:44:54.739933 pkscreener-0.44.20240319.246/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-03-19 06:40:40.000000 pkscreener-0.44.20240319.246/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 23:49:04.260328 pkscreener-0.44.20240405.248/
+-rw-rw-rw-   0        0        0     1086 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-05 23:49:04.260328 pkscreener-0.44.20240405.248/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 23:49:04.244711 pkscreener-0.44.20240405.248/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 23:49:04.260328 pkscreener-0.44.20240405.248/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27486 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    15888 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     7653 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    16886 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48873 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   108935 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    44525 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    77220 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-05 23:48:55.000000 pkscreener-0.44.20240405.248/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   108550 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    16667 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-05 23:49:04.244711 pkscreener-0.44.20240405.248/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-05 23:49:04.260328 pkscreener-0.44.20240405.248/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/setup.py
```

### Comparing `pkscreener-0.44.20240319.246/LICENSE` & `pkscreener-0.44.20240405.248/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/LICENSE-Others` & `pkscreener-0.44.20240405.248/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/PKG-INFO` & `pkscreener-0.44.20240405.248/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240319.246
+Version: 0.44.20240405.248
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240319.246.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240405.248.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240318.245/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240318.245/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240318.245/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240319.246/README.md` & `pkscreener-0.44.20240405.248/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240318.245/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240318.245/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240318.245/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240319.246/pkscreener/__init__.py` & `pkscreener-0.44.20240405.248/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/Fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,25 +27,27 @@
 import sys
 import warnings
 
 warnings.simplefilter("ignore", DeprecationWarning)
 warnings.simplefilter("ignore", FutureWarning)
 import pandas as pd
 import yfinance as yf
+from concurrent.futures import ThreadPoolExecutor
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.Fetcher import StockDataEmptyException
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.SuppressOutput import SuppressOutput
 from PKNSETools.PKNSEStockDataFetcher import nseStockDataFetcher
 from pkscreener.classes.PKTask import PKTask
 
 # This Class Handles Fetching of Stock Data over the internet
 
 
 class screenerStockDataFetcher(nseStockDataFetcher):
+    _tickersInfoDict={}
     def fetchStockDataWithArgs(self, *args):
         task = None
         if isinstance(args[0], PKTask):
             task = args[0]
             stockCode,period,duration,exchangeSuffix = task.long_running_fn_args
         else:
             stockCode,period,duration,exchangeSuffix = args[0],args[1],args[2],args[3]
@@ -54,15 +56,29 @@
             if task.taskId > 0:
                 task.progressStatusDict[task.taskId] = {'progress': 0, 'total': 1}
                 task.resultsDict[task.taskId] = result
                 task.progressStatusDict[task.taskId] = {'progress': 1, 'total': 1}
             else:
                 task.result = result
         return result
-    
+
+    def get_stats(self,ticker):
+        info = yf.Tickers(ticker).tickers[ticker].fast_info
+        screenerStockDataFetcher._tickersInfoDict[ticker] = {"marketCap":info.market_cap}
+
+    def fetchAdditionalTickerInfo(self,ticker_list,exchangeSuffix=".NS"):
+        if not isinstance(ticker_list,list):
+            raise TypeError("ticker_list must be a list")
+        if len(exchangeSuffix) > 0:
+            ticker_list = [(f"{x}{exchangeSuffix}" if not x.endswith(exchangeSuffix) else x) for x in ticker_list]
+        screenerStockDataFetcher._tickersInfoDict = {}
+        with ThreadPoolExecutor() as executor:
+            executor.map(self.get_stats, ticker_list)
+        return screenerStockDataFetcher._tickersInfoDict
+
     # Fetch stock price data from Yahoo finance
     def fetchStockData(
         self,
         stockCode,
         period,
         duration,
         proxyServer,
```

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,16 @@
     "1": "Buy Signals (Bullish Reversal)",
     "2": "Sell Signals (Bearish Reversal)",
     "3": "Momentum Gainers (Rising Bullish Momentum)",
     "4": "Reversal at Moving Average (Bullish Reversal)",
     "5": "Volume Spread Analysis (Bullish VSA Reversal)",
     "6": "Narrow Range (NRx) Reversal",
     "7": "Lorentzian Classifier (Machine Learning based indicator)",
+    "8": "PSAR and RSI reversal",
+    "9": "Rising RSI",
     "0": "Cancel",
 }
 level3_X_ChartPattern_MenuDict = {
     "1": "Bullish Inside Bar (Flag) Pattern",
     "2": "Bearish Inside Bar (Flag) Pattern(Sell)",
     "3": "The Confluence (50 & 200 MA/EMA)",
     "4": "VCP (Experimental)",
```

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/ScreeningStatistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -483,14 +483,55 @@
             saveDict["Breakout"] = saveDict["Breakout"] + "(Potential)"
             screenDict["Breakout"] = screenDict["Breakout"] + (
                 colorText.BOLD + colorText.GREEN + " (Potential)" + colorText.END
             )
             return True
         return False
 
+    # Find stocks with reversing PSAR and RSI
+    def findPSARReversalWithRSI(self, df, screenDict, saveDict,minRSI=50):
+        data = df.copy()
+        data = data[::-1]
+        psar = pktalib.psar(data["High"],data["Low"])
+        if len(psar) < 3:
+            return False
+        psar = psar.tail(3)
+        data = data.tail(3)
+        # dayMinus2Psar = psar.iloc[0]
+        dayMinus1Psar = psar.iloc[1]
+        dayPSAR = psar.iloc[2]
+        # dayMinus2Close = data["Close"].iloc[0]
+        dayMinus1Close = data["Close"].iloc[1]
+        dayClose = data["Close"].iloc[2]
+        # dayMinus2RSI = data["RSI"].iloc[0]
+        dayMinus1RSI = data["RSI"].iloc[1]
+        dayRSI = data["RSI"].iloc[2]
+        
+        hasReversal= (((dayMinus1Psar >= dayMinus1Close) and \
+                    (dayClose >= dayPSAR)) and \
+                    (dayMinus1RSI <= minRSI) and \
+                    (dayRSI >= dayMinus1RSI))
+        if hasReversal:
+            saved = self.findCurrentSavedValue(screenDict,saveDict, "Pattern")
+            screenDict["Pattern"] = (
+                saved[0] 
+                + colorText.BOLD
+                + colorText.GREEN
+                + f"PSAR-RSI-Rev"
+                + colorText.END
+            )
+            saveDict["Pattern"] = saved[1] + f"PSAR-RSI-Rev"
+                # (((dayMinus2Psar >= dayMinus2Close) and \
+                # ((dayMinus1Close >= dayMinus1Psar) and \
+                # (dayClose >= dayPSAR))) and \
+                # (dayMinus2RSI >= minRSI) and \
+                # (dayMinus1RSI >= dayMinus2RSI) and \
+                # (dayRSI >= dayMinus1RSI)) or \
+        return hasReversal
+
     # Find stock reversing at given MA
     def findReversalMA(self, df, screenDict, saveDict, maLength, percentage=0.02):
         data = df.copy()
         maRange = [10, 20, 50, 200]
         results = []
         hasReversals = False
         data = data[::-1]
@@ -609,15 +650,26 @@
             # Last 3 candles in squeeze
             if filter not in [2,4]: # SqZ/All
                 return False
             screenDict["Pattern"] = f'{saved[0]}{colorText.BOLD}{colorText.WARN}TTM-SQZ{colorText.END}'
             saveDict["Pattern"] = f'{saved[1]}TTM-SQZ'
             return True
         return False
-        
+
+    # Find stocks with rising RSI from lower levels
+    def findRisingRSI(self, df):
+        data = df.copy()
+        data = data[::-1]
+        data = data.tail(3)
+        dayMinus2RSI = data["RSI"].iloc[0]
+        dayMinus1RSI = data["RSI"].iloc[1]
+        dayRSI = data["RSI"].iloc[2]
+        return (dayMinus2RSI <= 35 and dayMinus1RSI > dayMinus2RSI and dayRSI > dayMinus1RSI) or \
+                (dayMinus1RSI <= 35 and dayRSI > dayMinus1RSI)
+
     #@measure_time
     # Find out trend for days to lookback
     def findTrend(self, df, screenDict, saveDict, daysToLookback=None, stockName=""):
         if df is None or len(df) == 0:
             return "Unknown"
         data = df.copy()
         if daysToLookback is None:
```

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/StockScreener.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,14 +147,16 @@
                 isMaReversal = 0
                 isIpoBase = False
                 isMaSupport = False
                 isLorentzian = False
                 isVCP = False
                 isVSA = False
                 isNR = False
+                hasPsarRSIReversal = False
+                hasRisingRSIReversal = False
                 isValidRsi = False
                 isBuyingTrendline = False
                 isMomentum = False
                 mfiStake = 0
                 fairValueDiff = 0
                 consolidationValue = 0
                 isBreaking = False
@@ -210,15 +212,28 @@
                 elif executeOption == 5:
                     isValidRsi = screener.validateRSI(
                         processedData, screeningDictionary, saveDictionary, minRSI, maxRSI
                     )
                     if not isValidRsi:
                         return returnLegibleData()
                 elif executeOption == 6:
-                    if reversalOption == 6:
+                    if reversalOption == 9:
+                        hasRisingRSIReversal = screener.findRisingRSI(processedData)
+                        if not hasRisingRSIReversal:
+                            return returnLegibleData()
+                    elif reversalOption == 8:
+                        hasPsarRSIReversal = screener.findPSARReversalWithRSI(
+                            processedData,
+                            screeningDictionary,
+                            saveDictionary
+                            # minRSI=maLength if maLength is not None else 40,
+                        )
+                        if not hasPsarRSIReversal:
+                            return returnLegibleData()
+                    elif reversalOption == 6:
                         isNR = screener.validateNarrowRange(
                             processedData,
                             screeningDictionary,
                             saveDictionary,
                             nr=maLength if maLength is not None else 4,
                         )
                         if not isNR:
@@ -408,14 +423,16 @@
                                                                     reversalOption == 5
                                                                     and isVSA
                                                                     and saveDictionary["Pattern"]
                                                                     in CandlePatterns.reversalPatternsBullish
                                                                 ))
                                                                 or (reversalOption == 6 and isNR)
                                                                 or (reversalOption == 7 and isLorentzian)
+                                                                or (reversalOption == 8 and hasPsarRSIReversal)
+                                                                or (reversalOption == 9 and hasRisingRSIReversal)
                                                                 ))
                         or ((executeOption == 7) and ((respChartPattern < 3 and isInsideBar > 0) 
                                                                   or (isConfluence)
                                                                   or (isIpoBase and newlyListedOnly and not respChartPattern < 3)
                                                                   or (isVCP)
                                                                   or (isBuyingTrendline))
                                                                   or (respChartPattern == 6 and hasBbandsSqz)
```

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1244,15 +1244,15 @@
                 input(
                     colorText.BOLD
                     + colorText.WARN
                     + """[+] Select Option:"""
                     + colorText.END
                 )
             )
-            if resp >= 0 and resp <= 7:
+            if resp >= 0 and resp <= 9:
                 if resp == 4:
                     try:
                         maLength = int(
                             input(
                                 colorText.BOLD
                                 + colorText.WARN
                                 + "\n[+] Enter MA Length (E.g. 50 or 200): "
```

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/classes/keys.py` & `pkscreener-0.44.20240405.248/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/courbd.ttf` & `pkscreener-0.44.20240405.248/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/globals.py` & `pkscreener-0.44.20240405.248/pkscreener/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -527,15 +527,15 @@
             Utility.tools.clearScreen()
             return initPostLevel1Execution(indexOption, executeOption, retrial=True)
     return indexOption, executeOption
 
 def labelDataForPrinting(screenResults, saveResults, configManager, volumeRatio,executeOption, reversalOption):
     # Publish to gSheet with https://github.com/burnash/gspread
     try:
-        sortKey = ["Volume"]
+        sortKey = ["%Chng"]
         ascending = [False]
         if executeOption == 21:
             if reversalOption in [3,5,6,7]:
                 sortKey = ["MFI"]
                 ascending = [reversalOption in [6,7]]
             elif reversalOption in [8,9]:
                 sortKey = ["FVDiff"]
@@ -1600,15 +1600,15 @@
     )
     pngName = f'PKS_{PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)}_{PKDateUtilities.currentDateTime().strftime("%d-%m-%y_%H.%M.%S")}'
     pngExtension = ".png"
     eligible = is_token_telegram_configured()
     targetDateG10k = prepareGrowthOf10kResults(saveResults, selectedChoice, menuChoiceHierarchy, testing, user, pngName, pngExtension, eligible)
     if saveResults is not None and "Date" in saveResults.columns and len(saveResults) > 0:
         recordDate = saveResults["Date"].iloc[0].replace("/","-")
-    removedUnusedColumns(screenResults, saveResults, ["Date","Breakout","Resistance"],userArgs=userPassedArgs)
+    summaryReturns = removedUnusedColumns(screenResults, saveResults, ["Date","Breakout","Resistance"],userArgs=userPassedArgs)
 
     tabulated_results = ""
     if screenResults is not None and len(screenResults) > 0:
         tabulated_results = colorText.miniTabulator().tabulate(
             screenResults, headers="keys", tablefmt=colorText.No_Pad_GridFormat,
             maxcolwidths=Utility.tools.getMaxColumnWidths(screenResults)
         ).encode("utf-8").decode(STD_ENCODING)
@@ -1720,15 +1720,15 @@
             else:
                 tabulateBacktestResults(saveResults)
         else:
             tabulateBacktestResults(saveResults)
             print(
                 colorText.BOLD
                 + colorText.GREEN
-                + f"[+] Found {len(screenResults) if screenResults is not None else 0} Stocks in {str('{:.2f}'.format(elapsed_time))} sec."
+                + f"[+] Found {len(screenResults) if screenResults is not None else 0} Stocks in {str('{:.2f}'.format(elapsed_time))} sec.{(' with portfolio returns:' + summaryReturns) if len(summaryReturns) > 0 else ''}"
                 + colorText.END
             )
     elif user is not None:
         sendMessageToTelegramChannel(
             message=f"No scan results found for {menuChoiceHierarchy}", user=user
         )
     if not testing:
@@ -1775,29 +1775,35 @@
     return targetDateG10k
 
 
 def removedUnusedColumns(screenResults, saveResults, dropAdditionalColumns=[], userArgs=None):
     periods = configManager.periodsRange
     if userArgs is not None and userArgs.backtestdaysago is not None and int(userArgs.backtestdaysago) < 22:
         dropAdditionalColumns.append("22-Pd %")
+    summaryReturns = ("w.r.t. " + saveResults["Date"].iloc[0]) if "Date" in saveResults.columns else ""
     for period in periods:
         if saveResults is not None:
+            if f"LTP{period}" in saveResults.columns:
+                pdReturn = round((sum(saveResults[f"LTP{period}"]) - sum(saveResults['LTP']))*100/sum(saveResults['LTP']),1)
+                if pdReturn > -500:
+                    summaryReturns = f"{period}-Pd({pdReturn} %), {summaryReturns}"
             saveResults.drop(f"LTP{period}", axis=1, inplace=True, errors="ignore")
             saveResults.drop(f"Growth{period}", axis=1, inplace=True, errors="ignore")
             if len(dropAdditionalColumns) > 0:
                 for col in dropAdditionalColumns:
                     if col in saveResults.columns:
                         saveResults.drop(col, axis=1, inplace=True, errors="ignore")
         if screenResults is not None:
             screenResults.drop(f"LTP{period}", axis=1, inplace=True, errors="ignore")
             screenResults.drop(f"Growth{period}", axis=1, inplace=True, errors="ignore")
             if len(dropAdditionalColumns) > 0:
                 for col in dropAdditionalColumns:
                     if col in screenResults.columns:
                         screenResults.drop(col, axis=1, inplace=True, errors="ignore")
+    return summaryReturns
 
 
 def tabulateBacktestResults(saveResults, maxAllowed=0, force=False):
     if "PKDevTools_Default_Log_Level" not in os.environ.keys():
         if ("RUNNER" not in os.environ.keys()) or ("RUNNER" in os.environ.keys() and not force) or not configManager.showPastStrategyData:
             return None, None
     tabulated_backtest_summary = ""
```

### Comparing `pkscreener-0.44.20240319.246/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240405.248/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240405.248/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240405.248/pkscreener/pkscreenercli.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,14 +152,19 @@
 )
 argParser.add_argument(
     "--maxdisplayresults",
     help="Maximum number of results to display.",
     required=False,
 )
 argParser.add_argument(
+    "--maxprice",
+    help="Maximum Price for the stock to be considered.",
+    required=False,
+)
+argParser.add_argument(
     "-o",
     "--options",
     help="Pass selected options in the <MainMenu>:<SubMenu>:<SubMenu>:etc. format. For example: ./pkscreenercli.py -a Y -o X:12:10 -e will run the screener with answer Y as default choice to questions and scan with menu choices: Scanners > Nifty (All Stocks) > Closing at least 2%% up since last 3 day",
     required=False,
 )
 argParser.add_argument(
     "-p",
@@ -341,15 +346,18 @@
     if args.intraday:
         configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
     else:
         configManager.toggleConfig(candleDuration='1d', clearCache=False)
     if args.options is not None and str(args.options) == "0":
         # Must be from unit tests to be able to break out of loops via eventing
         args.options = None
-
+    
+    if args.maxprice:
+        configManager.maxLTP = args.maxprice
+        configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
     if args.testbuild and not args.prodbuild:
         print(
             colorText.BOLD
             + colorText.FAIL
             + "[+] Started in TestBuild mode!"
             + colorText.END
         )
```

### Comparing `pkscreener-0.44.20240319.246/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240405.248/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240319.246
+Version: 0.44.20240405.248
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240319.246.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240405.248.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240318.245/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240318.245/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240318.245/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240319.246/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240405.248/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240319.246/setup.py` & `pkscreener-0.44.20240405.248/setup.py`

 * *Files identical despite different names*

