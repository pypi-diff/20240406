# Comparing `tmp/monsgrams-1.1.tar.gz` & `tmp/monsgrams-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsgrams-1.1.tar", last modified: Fri Apr  5 04:54:30 2024, max compression
+gzip compressed data, was "monsgrams-1.2.tar", last modified: Sat Apr  6 20:00:38 2024, max compression
```

## Comparing `monsgrams-1.1.tar` & `monsgrams-1.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 04:54:30.786729 monsgrams-1.1/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)     1118 2024-04-05 04:54:30.786729 monsgrams-1.1/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      852 2024-04-05 04:52:16.000000 monsgrams-1.1/README.md
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 04:54:30.770729 monsgrams-1.1/monsgrams/
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       20 2024-04-05 04:49:36.000000 monsgrams-1.1/monsgrams/__init__.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)     4013 2024-04-05 04:49:25.000000 monsgrams-1.1/monsgrams/bot.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 04:54:30.782729 monsgrams-1.1/monsgrams.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)     1118 2024-04-05 04:54:30.000000 monsgrams-1.1/monsgrams.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      221 2024-04-05 04:54:30.000000 monsgrams-1.1/monsgrams.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-05 04:54:30.000000 monsgrams-1.1/monsgrams.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       15 2024-04-05 04:54:30.000000 monsgrams-1.1/monsgrams.egg-info/requires.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-05 04:54:30.000000 monsgrams-1.1/monsgrams.egg-info/top_level.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-05 04:54:30.786729 monsgrams-1.1/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      443 2024-04-05 04:54:22.000000 monsgrams-1.1/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-06 20:00:38.665761 monsgrams-1.2/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      647 2024-04-06 20:00:38.665761 monsgrams-1.2/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      381 2024-04-06 19:59:48.000000 monsgrams-1.2/README.md
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-06 20:00:38.649761 monsgrams-1.2/monsgrams/
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       93 2024-04-06 16:25:30.000000 monsgrams-1.2/monsgrams/__init__.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      423 2024-04-06 06:37:09.000000 monsgrams-1.2/monsgrams/api.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       93 2024-04-06 15:07:16.000000 monsgrams-1.2/monsgrams/base.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     1237 2024-04-06 17:33:22.000000 monsgrams-1.2/monsgrams/bot.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     2530 2024-04-06 19:52:04.000000 monsgrams-1.2/monsgrams/message.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-06 20:00:38.661761 monsgrams-1.2/monsgrams.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      647 2024-04-06 20:00:38.000000 monsgrams-1.2/monsgrams.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      277 2024-04-06 20:00:38.000000 monsgrams-1.2/monsgrams.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-06 20:00:38.000000 monsgrams-1.2/monsgrams.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       15 2024-04-06 20:00:38.000000 monsgrams-1.2/monsgrams.egg-info/requires.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-06 20:00:38.000000 monsgrams-1.2/monsgrams.egg-info/top_level.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-06 20:00:38.665761 monsgrams-1.2/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      443 2024-04-06 19:59:59.000000 monsgrams-1.2/setup.py
```

