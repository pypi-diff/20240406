# Comparing `tmp/ObjectToString-0.2.65.tar.gz` & `tmp/ObjectToString-0.2.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ObjectToString-0.2.65.tar", last modified: Tue Apr  2 15:23:46 2024, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "ObjectToString-0.2.66.tar", last modified: Sat Apr  6 16:09:56 2024, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `ObjectToString-0.2.65.tar` & `ObjectToString-0.2.66.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-09-03 09:43:44.000000 ObjectToString-0.2.65/
--rw-rw-rw-   0        0        0       59 2023-09-03 09:39:02.000000 ObjectToString-0.2.65/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.65/objecttostring/
-drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.65/ObjectToString.egg-info/
--rw-rw-rw-   0        0        0        1 2023-09-06 15:34:55.000000 ObjectToString-0.2.65/ObjectToString.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-09-06 15:34:55.000000 ObjectToString-0.2.65/ObjectToString.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-09-06 15:34:55.000000 ObjectToString-0.2.65/ObjectToString.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2023-09-06 15:34:55.000000 ObjectToString-0.2.65/ObjectToString.egg-info/top_level.txt
--rwxrwxrwx   0        0        0  3702272 2024-04-02 15:00:53.000000 ObjectToString-0.2.65/objecttostring/pdslib.cp312-win_amd64.pyd
--rwxrwxrwx   0        0        0     4368 2024-02-22 15:49:50.000000 ObjectToString-0.2.65/objecttostring/test1.py
--rwxrwxrwx   0        0        0      100 2024-04-02 15:23:40.000000 ObjectToString-0.2.65/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-09-06 15:34:56.000000 ObjectToString-0.2.65/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-09-03 09:43:44.000000 ObjectToString-0.2.65/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-03 09:43:44.000000 ObjectToString-0.2.66/
+-rw-rw-rw-   0        0        0       59 2023-09-03 09:39:02.000000 ObjectToString-0.2.66/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.66/objecttostring/
+drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.66/ObjectToString.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-09-06 15:34:55.000000 ObjectToString-0.2.66/ObjectToString.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-09-06 15:34:55.000000 ObjectToString-0.2.66/ObjectToString.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-09-06 15:34:55.000000 ObjectToString-0.2.66/ObjectToString.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       15 2023-09-06 15:34:55.000000 ObjectToString-0.2.66/ObjectToString.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0  3702784 2024-04-06 15:56:26.000000 ObjectToString-0.2.66/objecttostring/pdslib.cp312-win_amd64.pyd
+-rwxrwxrwx   0        0        0   138240 2024-04-06 15:24:12.000000 ObjectToString-0.2.66/objecttostring/python.exe
+-rwxrwxrwx   0        0        0    56320 2024-04-06 15:24:07.000000 ObjectToString-0.2.66/objecttostring/python3.dll
+-rwxrwxrwx   0        0        0  9321472 2024-04-06 15:24:12.000000 ObjectToString-0.2.66/objecttostring/python312.dll
+-rwxrwxrwx   0        0        0     4368 2024-02-22 15:49:50.000000 ObjectToString-0.2.66/objecttostring/test1.py
+-rwxrwxrwx   0        0        0      100 2024-04-06 16:09:51.000000 ObjectToString-0.2.66/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-09-06 15:34:56.000000 ObjectToString-0.2.66/setup.cfg
+-rw-rw-rw-   0        0        0      234 2023-09-03 09:43:44.000000 ObjectToString-0.2.66/setup.py
```

### Comparing `ObjectToString-0.2.65/objecttostring/test1.py` & `ObjectToString-0.2.66/objecttostring/test1.py`

 * *Files identical despite different names*

