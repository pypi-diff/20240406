# Comparing `tmp/Mopidy-SevenSegmentDisplay-0.7.3.tar.gz` & `tmp/Mopidy-SevenSegmentDisplay-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mopidy-SevenSegmentDisplay-0.7.3.tar", last modified: Sat Mar 23 12:10:04 2024, max compression
+gzip compressed data, was "Mopidy-SevenSegmentDisplay-0.7.4.tar", last modified: Sat Apr  6 16:47:18 2024, max compression
```

## Comparing `Mopidy-SevenSegmentDisplay-0.7.3.tar` & `Mopidy-SevenSegmentDisplay-0.7.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:10:04.203066 Mopidy-SevenSegmentDisplay-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:10:04.203066 Mopidy-SevenSegmentDisplay-0.7.3/Mopidy_SevenSegmentDisplay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-23 12:10:04.000000 Mopidy-SevenSegmentDisplay-0.7.3/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-23 12:10:04.000000 Mopidy-SevenSegmentDisplay-0.7.3/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 12:10:04.000000 Mopidy-SevenSegmentDisplay-0.7.3/Mopidy_SevenSegmentDisplay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-23 12:10:04.000000 Mopidy-SevenSegmentDisplay-0.7.3/Mopidy_SevenSegmentDisplay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 12:10:04.000000 Mopidy-SevenSegmentDisplay-0.7.3/Mopidy_SevenSegmentDisplay.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-23 12:10:04.000000 Mopidy-SevenSegmentDisplay-0.7.3/Mopidy_SevenSegmentDisplay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-23 12:10:04.000000 Mopidy-SevenSegmentDisplay-0.7.3/Mopidy_SevenSegmentDisplay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-23 12:10:04.203066 Mopidy-SevenSegmentDisplay-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:10:04.199066 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/cava.config
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/equalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/ext.conf
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/led.py
--rw-r--r--   0 runner    (1001) docker     (127)    25861 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/lib_nrf24.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/light_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/max7219.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/music.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:10:04.203066 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/alwan.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/alwan.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)   109518 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    31819 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:10:04.203066 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-23 12:10:04.203066 Mopidy-SevenSegmentDisplay-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-23 12:09:59.000000 Mopidy-SevenSegmentDisplay-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:47:18.896524 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/cava.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/equalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/ext.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25861 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/lib_nrf24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/light_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/max7219.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/music.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/alwan.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/alwan.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)   109518 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    31819 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/setup.py
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/LICENSE` & `Mopidy-SevenSegmentDisplay-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO` & `Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-SevenSegmentDisplay
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Mopidy extension for using it with seven segment display.
 Home-page: https://github.com/JumalIO/mopidy-sevensegmentdisplay
 Author: Julius
 Author-email: spamjulius@mail.com
 Maintainer: Julius
 Maintainer-email: spamjulius@mail.com
 License: Apache License, Version 2.0
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt` & `Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/PKG-INFO` & `Mopidy-SevenSegmentDisplay-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-SevenSegmentDisplay
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Mopidy extension for using it with seven segment display.
 Home-page: https://github.com/JumalIO/mopidy-sevensegmentdisplay
 Author: Julius
 Author-email: spamjulius@mail.com
 Maintainer: Julius
 Maintainer-email: spamjulius@mail.com
 License: Apache License, Version 2.0
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/README.md` & `Mopidy-SevenSegmentDisplay-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/__init__.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from mopidy import config, ext
 from .http import factory_decorator
 from .actor import Frontend
 
-__version__ = '0.7.3'
+__version__ = '0.7.4'
 
 
 class Extension(ext.Extension):
     dist_name = 'Mopidy-SevenSegmentDisplay'
     ext_name = 'sevensegmentdisplay'
     version = __version__
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/actor.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/actor.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/alert.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/alert.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/animation.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/animation.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/clock.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/clock.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/display.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/display.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/equalizer.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/equalizer.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/ext.conf` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/ext.conf`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/gpio.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/gpio.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/http.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/http.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/ir.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/ir.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/led.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/led.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,65 +4,94 @@
 import RPi.GPIO as GPIO
 from .lib_nrf24 import NRF24
 
 
 class Led:
     
     def __init__(self, led_enabled):
-        self._spi = None
         self._radio = None
+        self._pipes = []
+        self._size = 8
 
         if (not led_enabled):
             return
 
         GPIO.setmode(GPIO.BCM)
-
-        pipes = [[0xE0, 0xE0, 0xF1, 0xF1, 0xE0], [0xF1, 0xF1, 0xF0, 0xF0, 0xE0]]
+        
+        readingPipe = [0xF0, 0xF0, 0xF0, 0xF0, 0xE1]
 
         import spidev
-        self._spi = spidev.SpiDev()
-        self._spi.open(0, 1)
-        self._spi.cshigh = False
-        self._spi.max_speed_hz = 500000
-        self._spi.mode = 0
+        spi = spidev.SpiDev()
+        spi.open(0, 1)
+        spi.cshigh = False
+        spi.max_speed_hz = 500000
+        spi.mode = 0
 
-        self._radio = NRF24(GPIO, self._spi)
+        self._radio = NRF24(GPIO, spi)
         self._radio.begin(1, 25)
-        self._radio.setPayloadSize(8)
-        self._radio.setChannel(0x7A)
+
+        self._radio.setPayloadSize(self._size)
+        self._radio.setChannel(0x76)
         self._radio.setDataRate(NRF24.BR_1MBPS)
-        self._radio.setPALevel(NRF24.PA_MIN)
+        self._radio.setPALevel(NRF24.PA_MAX)
         self._radio.setAutoAck(True)
-        self._radio.openWritingPipe(pipes[0])
-        self._radio.openReadingPipe(1, pipes[1])
+        self._radio.openReadingPipe(1, readingPipe)
         self._radio.printDetails()
 
-    def setColor(self, red, green, blue):
-        if self._radio is None:
-            return
+        self._radio.startListening()
+
+    def run(self):
+        if self._radio.available():
+            r = []
+
+            self._radio.read(r, self._size)
+
+            logging.info(r)
 
-        self._radio.write([0, red, green, blue])
+            if (r[0] != 1):
+                return
 
-        if self._radio.isAckPayloadAvailable():
-            buffer = []
-            self._radio.read(buffer, self._radio.getDynamicPayloadSize())
-            logging.info("NRF24 ACK Received:"),
-            logging.info(buffer)
-        else:
-            logging.info("Received: Ack only, no payload")
+            for pipe in self._pipes:
+                if (pipe[0] == r[1] and
+                    pipe[1] == r[2] and
+                    pipe[2] == r[3] and
+                    pipe[3] == r[4] and
+                    pipe[4] == r[5]):
+                    return
+
+            self._pipes.append([r[1], r[2], r[3], r[4], r[5]])
+
+
+    def setColor(self, red, green, blue):
+        try:
+            if self._radio is None:
+                return
+
+            self._radio.stopListening()
+
+            for pipe in self._pipes:
+                self._radio.openWritingPipe(pipe);
+
+                self._radio.write([0, red, green, blue])
+
+                if self._radio.isAckPayloadAvailable():
+                    buffer = []
+                    self._radio.read(buffer, self._radio.getDynamicPayloadSize())
+                    logging.info("NRF24 ACK Received:"),
+                    logging.info(buffer)
+                else:
+                    logging.info("Received: Ack only, no payload")
+
+            self._radio.startListening()
+        except Exception as inst:
+            logging.error(inst)
         
     def setColorHsv(self, hue, sat = 1, val = 1):
         c = colorsys.hsv_to_rgb(hue / 360.0, sat, val)
             
         self.setColor(int(c[0] * 255), int(c[1] * 255), int(c[2] * 255))
 
     def setRandomColor(self):
         self.setColorHsv(random.random() * 360)
 
     def setNoneColor(self):
         self.setColor(0, 0, 0)
-        
-    def stop(self):
-        if self._spi is None:
-            return
-        
-        self._spi.close()
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/lib_nrf24.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/lib_nrf24.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/light_sensor.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/light_sensor.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/max7219.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/max7219.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/menu.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/menu.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/music.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/music.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/alwan.min.css` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/alwan.min.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/alwan.min.js` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/alwan.min.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/bootstrap-theme.css` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/bootstrap.css` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/bootstrap.js` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/static/jquery.js` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/jquery.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/templates/base.html` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/templates/base.html`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/templates/index.html` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/templates/index.html`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/timer.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/timer.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/mopidy_sevensegmentdisplay/worker.py` & `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,23 +80,23 @@
                     break
 
                 if (self.equalizer.is_visible() and not self.menu.is_sub_menu_visible()):
                     self.equalizer.run()
                 else:
                     self.equalizer.stop()
                     self.menu.run()
+                    self.led.run()
                     sleep(1)
 
         except Exception as inst:
             logging.error(inst)
         finally:
             self.equalizer.stop()
             self.ir_sender.stop()
             self.led.setNoneColor()
-            self.led.stop()
             self.gpio.cleanup()
             self.display.stop()
             self.light_sensor.stop()
 
     def _init_menu(self):
         self.MENU = {
             "get_sub_menu": lambda: [
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.3/setup.py` & `Mopidy-SevenSegmentDisplay-0.7.4/setup.py`

 * *Files identical despite different names*

