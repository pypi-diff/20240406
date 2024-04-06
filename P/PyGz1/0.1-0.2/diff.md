# Comparing `tmp/PyGz1-0.1.tar.gz` & `tmp/PyGz1-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGz1-0.1.tar", last modified: Sat Apr  6 10:53:58 2024, max compression
+gzip compressed data, was "PyGz1-0.2.tar", last modified: Sat Apr  6 13:43:52 2024, max compression
```

## Comparing `PyGz1-0.1.tar` & `PyGz1-0.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 10:53:58.531636 PyGz1-0.1/
--rw-rw-rw-   0        0        0      161 2024-04-06 10:53:58.530635 PyGz1-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 10:53:58.528637 PyGz1-0.1/PyGz1.egg-info/
--rw-rw-rw-   0        0        0      161 2024-04-06 10:53:58.000000 PyGz1-0.1/PyGz1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2024-04-06 10:53:58.000000 PyGz1-0.1/PyGz1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 10:53:58.000000 PyGz1-0.1/PyGz1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 10:53:58.000000 PyGz1-0.1/PyGz1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-06 10:53:58.000000 PyGz1-0.1/PyGz1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 10:53:58.532635 PyGz1-0.1/setup.cfg
--rw-rw-rw-   0        0        0      274 2024-04-05 18:09:16.000000 PyGz1-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:43:52.711764 PyGz1-0.2/
+-rw-rw-rw-   0        0        0      161 2024-04-06 13:43:52.710780 PyGz1-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 13:43:52.704504 PyGz1-0.2/PyGz1.egg-info/
+-rw-rw-rw-   0        0        0      161 2024-04-06 13:43:52.000000 PyGz1-0.2/PyGz1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-06 13:43:52.000000 PyGz1-0.2/PyGz1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 13:43:52.000000 PyGz1-0.2/PyGz1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 13:43:52.000000 PyGz1-0.2/PyGz1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-06 13:43:52.000000 PyGz1-0.2/PyGz1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 13:43:52.709749 PyGz1-0.2/pygz1/
+-rw-rw-rw-   0        0        0      425 2024-04-06 13:40:22.000000 PyGz1-0.2/pygz1/__init__.py
+-rw-rw-rw-   0        0        0      769 2024-04-06 13:38:18.000000 PyGz1-0.2/pygz1/network.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 13:36:44.000000 PyGz1-0.2/pygz1/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-06 13:43:52.711764 PyGz1-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      274 2024-04-06 13:42:42.000000 PyGz1-0.2/setup.py
```

