# Comparing `tmp/PyGz1-0.3.1.tar.gz` & `tmp/PyGz1-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGz1-0.3.1.tar", last modified: Sat Apr  6 14:17:20 2024, max compression
+gzip compressed data, was "PyGz1-0.3.2.tar", last modified: Sat Apr  6 14:47:04 2024, max compression
```

## Comparing `PyGz1-0.3.1.tar` & `PyGz1-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 14:17:20.989488 PyGz1-0.3.1/
--rw-rw-rw-   0        0        0      163 2024-04-06 14:17:20.977641 PyGz1-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 14:17:20.970646 PyGz1-0.3.1/PyGz1.egg-info/
--rw-rw-rw-   0        0        0      163 2024-04-06 14:17:20.000000 PyGz1-0.3.1/PyGz1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-06 14:17:20.000000 PyGz1-0.3.1/PyGz1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 14:17:20.000000 PyGz1-0.3.1/PyGz1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 14:17:20.000000 PyGz1-0.3.1/PyGz1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-06 14:17:20.000000 PyGz1-0.3.1/PyGz1.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 14:17:20.974626 PyGz1-0.3.1/pygz1/
--rw-rw-rw-   0        0        0      729 2024-04-06 14:11:13.000000 PyGz1-0.3.1/pygz1/__init__.py
--rw-rw-rw-   0        0        0     3208 2024-04-06 14:09:16.000000 PyGz1-0.3.1/pygz1/network.py
--rw-rw-rw-   0        0        0        0 2024-04-06 13:36:44.000000 PyGz1-0.3.1/pygz1/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-06 14:17:20.989488 PyGz1-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      276 2024-04-06 14:17:12.000000 PyGz1-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:47:04.352119 PyGz1-0.3.2/
+-rw-rw-rw-   0        0        0      163 2024-04-06 14:47:04.351117 PyGz1-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 14:47:04.344083 PyGz1-0.3.2/PyGz1.egg-info/
+-rw-rw-rw-   0        0        0      163 2024-04-06 14:47:04.000000 PyGz1-0.3.2/PyGz1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-06 14:47:04.000000 PyGz1-0.3.2/PyGz1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 14:47:04.000000 PyGz1-0.3.2/PyGz1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 14:47:04.000000 PyGz1-0.3.2/PyGz1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-06 14:47:04.000000 PyGz1-0.3.2/PyGz1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      377 2024-04-06 14:46:45.000000 PyGz1-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 14:47:04.349095 PyGz1-0.3.2/pygz1/
+-rw-rw-rw-   0        0        0      729 2024-04-06 14:11:13.000000 PyGz1-0.3.2/pygz1/__init__.py
+-rw-rw-rw-   0        0        0     3208 2024-04-06 14:09:16.000000 PyGz1-0.3.2/pygz1/network.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 13:36:44.000000 PyGz1-0.3.2/pygz1/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-06 14:47:04.353124 PyGz1-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      276 2024-04-06 14:46:56.000000 PyGz1-0.3.2/setup.py
```

### Comparing `PyGz1-0.3.1/pygz1/__init__.py` & `PyGz1-0.3.2/pygz1/__init__.py`

 * *Files identical despite different names*

### Comparing `PyGz1-0.3.1/pygz1/network.py` & `PyGz1-0.3.2/pygz1/network.py`

 * *Files identical despite different names*

