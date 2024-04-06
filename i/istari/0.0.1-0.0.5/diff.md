# Comparing `tmp/istari-0.0.1.tar.gz` & `tmp/istari-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istari-0.0.1.tar", last modified: Wed Mar 27 20:21:38 2024, max compression
+gzip compressed data, was "istari-0.0.5.tar", last modified: Sat Apr  6 03:57:17 2024, max compression
```

## Comparing `istari-0.0.1.tar` & `istari-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,30 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-03-27 20:21:38.339899 istari-0.0.1/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-03-27 20:21:38.339747 istari-0.0.1/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      106 2024-03-27 20:20:38.000000 istari-0.0.1/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-03-27 20:21:38.338893 istari-0.0.1/istari/
--rw-r--r--   0 jay        (501) staff       (20)       22 2024-03-27 20:20:08.000000 istari-0.0.1/istari/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-03-27 20:21:38.339575 istari-0.0.1/istari/cli/
--rw-r--r--   0 jay        (501) staff       (20)       37 2024-03-27 20:11:49.000000 istari-0.0.1/istari/cli/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-03-27 20:21:38.339459 istari-0.0.1/istari.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-03-27 20:21:38.000000 istari-0.0.1/istari.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      213 2024-03-27 20:21:38.000000 istari-0.0.1/istari.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2024-03-27 20:21:38.000000 istari-0.0.1/istari.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       43 2024-03-27 20:21:38.000000 istari-0.0.1/istari.egg-info/entry_points.txt
--rw-r--r--   0 jay        (501) staff       (20)        7 2024-03-27 20:21:38.000000 istari-0.0.1/istari.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)       38 2024-03-27 20:21:38.339935 istari-0.0.1/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      459 2024-03-27 20:19:15.000000 istari-0.0.1/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 03:57:17.975136 istari-0.0.5/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-06 03:57:17.974968 istari-0.0.5/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.0.5/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 03:57:17.972882 istari-0.0.5/istari/
+-rw-r--r--   0 jay        (501) staff       (20)      292 2024-04-06 03:53:21.000000 istari-0.0.5/istari/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 03:57:17.973586 istari-0.0.5/istari/auth/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.0.5/istari/auth/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3022 2024-04-06 03:42:22.000000 istari-0.0.5/istari/auth/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 03:57:17.973801 istari-0.0.5/istari/cli/
+-rw-r--r--   0 jay        (501) staff       (20)     1450 2024-04-05 21:17:27.000000 istari-0.0.5/istari/cli/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.0.5/istari/cli/commands.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 03:57:17.974113 istari-0.0.5/istari/commands/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.0.5/istari/commands/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      929 2024-04-06 02:58:34.000000 istari-0.0.5/istari/commands/startapp.py
+-rw-r--r--   0 jay        (501) staff       (20)      629 2024-04-06 02:20:21.000000 istari-0.0.5/istari/commands/startproject.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 03:57:17.974471 istari-0.0.5/istari/db/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.0.5/istari/db/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.0.5/istari/db/fields.py
+-rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-06 00:40:42.000000 istari-0.0.5/istari/db/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 03:57:17.974677 istari-0.0.5/istari/templates/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 02:02:06.000000 istari-0.0.5/istari/templates/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     2639 2024-04-06 02:36:09.000000 istari-0.0.5/istari/templates/commands.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 03:57:17.973404 istari-0.0.5/istari.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-06 03:57:17.000000 istari-0.0.5/istari.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      490 2024-04-06 03:57:17.000000 istari-0.0.5/istari.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-06 03:57:17.000000 istari-0.0.5/istari.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-06 03:57:17.000000 istari-0.0.5/istari.egg-info/entry_points.txt
+-rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-06 03:57:17.000000 istari-0.0.5/istari.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-06 03:57:17.975166 istari-0.0.5/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.0.5/setup.py
```

