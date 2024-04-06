# Comparing `tmp/CnbcNews-0.3.tar.gz` & `tmp/CnbcNews-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CnbcNews-0.3.tar", last modified: Sat Apr  6 14:29:46 2024, max compression
+gzip compressed data, was "CnbcNews-1.0.tar", last modified: Sat Apr  6 14:33:12 2024, max compression
```

## Comparing `CnbcNews-0.3.tar` & `CnbcNews-1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 14:29:46.124984 CnbcNews-0.3/
-drwxrwxrwx   0        0        0        0 2024-04-06 14:29:46.089634 CnbcNews-0.3/CnbcNews/
--rw-rw-rw-   0        0        0       29 2024-04-06 14:05:57.000000 CnbcNews-0.3/CnbcNews/__init__.py
--rw-rw-rw-   0        0        0     3734 2024-04-06 14:29:26.000000 CnbcNews-0.3/CnbcNews/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 14:29:46.118662 CnbcNews-0.3/CnbcNews.egg-info/
--rw-rw-rw-   0        0        0       53 2024-04-06 14:29:45.000000 CnbcNews-0.3/CnbcNews.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-04-06 14:29:45.000000 CnbcNews-0.3/CnbcNews.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 14:29:45.000000 CnbcNews-0.3/CnbcNews.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 14:29:45.000000 CnbcNews-0.3/CnbcNews.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       53 2024-04-06 14:29:46.122818 CnbcNews-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-06 14:05:09.000000 CnbcNews-0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 14:29:46.125997 CnbcNews-0.3/setup.cfg
--rw-rw-rw-   0        0        0      205 2024-04-06 14:29:40.000000 CnbcNews-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:33:12.723647 CnbcNews-1.0/
+drwxrwxrwx   0        0        0        0 2024-04-06 14:33:12.688061 CnbcNews-1.0/CnbcNews/
+-rw-rw-rw-   0        0        0       29 2024-04-06 14:05:57.000000 CnbcNews-1.0/CnbcNews/__init__.py
+-rw-rw-rw-   0        0        0     3734 2024-04-06 14:29:26.000000 CnbcNews-1.0/CnbcNews/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:33:12.718433 CnbcNews-1.0/CnbcNews.egg-info/
+-rw-rw-rw-   0        0        0       53 2024-04-06 14:33:12.000000 CnbcNews-1.0/CnbcNews.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-04-06 14:33:12.000000 CnbcNews-1.0/CnbcNews.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 14:33:12.000000 CnbcNews-1.0/CnbcNews.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-06 14:33:12.000000 CnbcNews-1.0/CnbcNews.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 14:33:12.000000 CnbcNews-1.0/CnbcNews.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       53 2024-04-06 14:33:12.721442 CnbcNews-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-06 14:05:09.000000 CnbcNews-1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 14:33:12.723647 CnbcNews-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      335 2024-04-06 14:33:02.000000 CnbcNews-1.0/setup.py
```

### Comparing `CnbcNews-0.3/CnbcNews/main.py` & `CnbcNews-1.0/CnbcNews/main.py`

 * *Files identical despite different names*

