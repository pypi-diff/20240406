# Comparing `tmp/PyGz1-0.2.tar.gz` & `tmp/PyGz1-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGz1-0.2.tar", last modified: Sat Apr  6 13:43:52 2024, max compression
+gzip compressed data, was "PyGz1-0.3.tar", last modified: Sat Apr  6 14:01:43 2024, max compression
```

## Comparing `PyGz1-0.2.tar` & `PyGz1-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 13:43:52.711764 PyGz1-0.2/
--rw-rw-rw-   0        0        0      161 2024-04-06 13:43:52.710780 PyGz1-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 13:43:52.704504 PyGz1-0.2/PyGz1.egg-info/
--rw-rw-rw-   0        0        0      161 2024-04-06 13:43:52.000000 PyGz1-0.2/PyGz1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-06 13:43:52.000000 PyGz1-0.2/PyGz1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 13:43:52.000000 PyGz1-0.2/PyGz1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 13:43:52.000000 PyGz1-0.2/PyGz1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-06 13:43:52.000000 PyGz1-0.2/PyGz1.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 13:43:52.709749 PyGz1-0.2/pygz1/
--rw-rw-rw-   0        0        0      425 2024-04-06 13:40:22.000000 PyGz1-0.2/pygz1/__init__.py
--rw-rw-rw-   0        0        0      769 2024-04-06 13:38:18.000000 PyGz1-0.2/pygz1/network.py
--rw-rw-rw-   0        0        0        0 2024-04-06 13:36:44.000000 PyGz1-0.2/pygz1/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-06 13:43:52.711764 PyGz1-0.2/setup.cfg
--rw-rw-rw-   0        0        0      274 2024-04-06 13:42:42.000000 PyGz1-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:01:43.470139 PyGz1-0.3/
+-rw-rw-rw-   0        0        0      161 2024-04-06 14:01:43.469157 PyGz1-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 14:01:43.462239 PyGz1-0.3/PyGz1.egg-info/
+-rw-rw-rw-   0        0        0      161 2024-04-06 14:01:43.000000 PyGz1-0.3/PyGz1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-06 14:01:43.000000 PyGz1-0.3/PyGz1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 14:01:43.000000 PyGz1-0.3/PyGz1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 14:01:43.000000 PyGz1-0.3/PyGz1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-06 14:01:43.000000 PyGz1-0.3/PyGz1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 14:01:43.468143 PyGz1-0.3/pygz1/
+-rw-rw-rw-   0        0        0      710 2024-04-06 13:57:14.000000 PyGz1-0.3/pygz1/__init__.py
+-rw-rw-rw-   0        0        0     3176 2024-04-06 13:56:44.000000 PyGz1-0.3/pygz1/network.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 13:36:44.000000 PyGz1-0.3/pygz1/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-06 14:01:43.470139 PyGz1-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      274 2024-04-06 13:57:19.000000 PyGz1-0.3/setup.py
```

